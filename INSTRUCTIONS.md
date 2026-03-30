# Instructions

## Setup Instructions

1. Open the project in your IDE (VSCode recommended)
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure the project (see Configuration section below)
4. Run the application:
   ```bash
   npm start
   ```

## Configuration

Create a configuration file (or update existing settings) with the following parameters:

### Account Settings
- **Development Account**: Use a dedicated Stack Overflow account for testing
- **Authentication**: Configure Stack Overflow credentials securely (environment variables recommended)
- **Session Management**: Handle cookies and session persistence

### Bot Behavior Settings
- **Vote Count**: Number of random votes per run (default: 20)
- **Target Tags**: Specific Stack Overflow tags to target for voting
- **Edit Count**: Number of posts to edit per run
- **Rate Limiting**: Delays between operations to avoid detection

### Spell Check Patterns
Configure patterns to detect spelling mistakes:
- Lowercase first letter in questions (outside code blocks)
- Common spelling mistakes
- Score calculation thresholds for multi-mistake posts

## Running Scripts

### Vote Script
Crawls Stack Overflow and casts votes on random questions with specific tags:
```bash
npm run vote
```

**What it does:**
- Authenticates with Stack Overflow
- Finds questions matching configured tags
- Randomly selects questions
- Casts upvotes/downvotes based on configuration
- Logs all actions

### Fix Script
Finds and fixes spelling mistakes on Stack Overflow posts:
```bash
npm run fix
```

**What it does:**
- Scans posts for spelling patterns
- Identifies mistakes outside code snippets
- Calculates score for multiple mistakes
- Suggests or applies edits
- Logs corrections made

### Daily Script
Combines voting and editing in a single daily run:
```bash
npm run daily
```

**What it does:**
- Performs configured number of votes (default: 20)
- Edits configured number of posts
- Respects rate limits
- Generates daily report

## Testing and Development

### Initial Testing Phase
Before running on production:
1. Create a development Stack Overflow account
2. Run the bot for 2-3 weeks on the test account
3. Verify no captcha challenges appear
4. Monitor for any blocks or warnings
5. Adjust rate limiting and delays as needed

### Debugging
- Enable verbose logging in configuration
- Check browser console for errors
- Review Puppeteer screenshots on failures
- Monitor network requests

## Important Notes

### Ethical Considerations
- This bot should only be used ethically and in compliance with Stack Overflow's terms of service
- Always test on development accounts first
- Implement proper rate limiting
- Respect captcha challenges
- Do not spam or abuse the platform

### Rate Limiting
- Add delays between operations (recommended: 5-10 seconds)
- Limit daily operations to reasonable numbers
- Monitor for rate limit errors
- Implement exponential backoff on failures

### Captcha Handling
- If captcha appears, stop automation
- Log captcha occurrences
- Adjust rate limiting parameters
- Consider longer delays between operations

## Maintenance

### Backup Before Changes
Always create a backup before making changes:
```bash
npm run backup
```

### Update Checklist
When making changes:
1. Perform backup
2. Test changes on development account
3. Update documentation if needed
4. Commit and push to Git repository
5. Update backups to external storage

## Troubleshooting

### Common Issues

**Authentication Failures:**
- Verify credentials are correct
- Check if cookies have expired
- Re-authenticate manually and capture new session

**Captcha Challenges:**
- Reduce operation frequency
- Increase delays between actions
- Consider human-like randomization

**Element Not Found:**
- Stack Overflow UI may have changed
- Update selectors in configuration
- Review page structure with browser dev tools

**Rate Limiting:**
- Reduce operations per run
- Increase delays
- Check Stack Overflow API limits

## Author

* **Or Assayag** - *Initial work* - [orassayag](https://github.com/orassayag)
* Or Assayag <orassayag@gmail.com>
* GitHub: https://github.com/orassayag
* StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
* LinkedIn: https://linkedin.com/in/orassayag
