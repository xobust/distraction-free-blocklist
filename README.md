# Distraction Free Blocklist - Stop Endless Scrolling

A uBlock Origin filter list designed to block social media feeds and infinite scroll content to help reduce screen time and improve productivity.

## 🎯 Purpose

This filter list targets the addictive feed interfaces of popular social media platforms while preserving access to important features like:

- Direct messages
- Single post view with comments
- Search functionality
- Profile pages
- Settings and navigation

## 📋 Supported Platforms

- **Facebook** - Blocks news feed and story content
- **Instagram** - Blocks post feed and explore content
- **Twitter/X** - Blocks tweet feed and trending content
- **Reddit** - Blocks post feed and subreddit content
- **TikTok** - Blocks video feed and recommended content
- **YouTube** - Blocks video recommendations and trending
- **LinkedIn** - Blocks feed posts and updates
- **Pinterest** - Blocks pin feed and recommendations
- **Snapchat** - Blocks story feed and discover content

## 🚀 Installation

### Prerequisites

**Recommended Setup:**

- **Browser**: Firefox (best privacy and uBlock Origin support)
- **Extension**: uBlock Origin (not uBlock - the original uBlock Origin by gorhill)

**Why Firefox + uBlock Origin?**

- Firefox has the best privacy features and extension support
- uBlock Origin is the most powerful and actively maintained ad blocker
- Better performance and fewer conflicts with other extensions
- Regular updates and strong community support

**⚠️ Important**: Make sure you install "uBlock Origin" (by gorhill), not "uBlock" (different extension). The correct extension has "Origin" in the name.

### Method 1: Direct Import (Recommended)

1. Install [uBlock Origin](https://github.com/gorhill/uBlock) in Firefox (recommended) or your preferred browser
2. Open uBlock Origin settings
3. Go to the "Filter lists" tab
4. Click "Import" and paste this URL:
   ```
   https://raw.githubusercontent.com/xobust/distraction-free-blocklist/main/distraction-free-blocklist.txt
   ```
5. Click "Apply changes"

### Method 2: Manual Import

1. Download the `distraction-free-blocklist.txt` file from this repository
2. Open uBlock Origin settings
3. Go to the "Filter lists" tab
4. Click "Import" and select the downloaded file
5. Click "Apply changes"

### Method 3: Subscribe to Filter List

1. Open uBlock Origin settings
2. Go to the "Filter lists" tab
3. Scroll down to "Custom" section
4. Click the "+" button
5. Add the filter list URL and give it a name like "Distraction Free Blocklist"

## ⚙️ Configuration

### Customization

You can customize the filter list by editing `distraction-free-blocklist.txt`:

- **Remove specific platforms**: Delete the sections for platforms you want to keep
- **Add new platforms**: Follow the existing pattern to add new social media sites
- **Adjust blocking level**: Modify selectors to be more or less aggressive

### Whitelist Rules

The filter list includes whitelist rules (`#@#`) to preserve important functionality:

- Search results
- Profile pages
- Direct messaging
- Navigation menus
- Settings pages

## 🔧 Troubleshooting

### Common Issues

1. **Too aggressive blocking**: Some legitimate content might be blocked

   - Solution: Add whitelist rules for specific elements you need

2. **Not blocking enough**: Some feed content still appears

   - Solution: Social media sites frequently change their selectors
   - Check for updates to the filter list

3. **Breaking website functionality**: Important features stop working
   - Solution: Check the whitelist rules or temporarily disable the filter

### Testing

To test if the filter list is working:

1. Visit a social media site (e.g., facebook.com)
2. Look for the main feed area - it should be blocked or significantly reduced
3. Check that navigation and messaging still work

## 📝 Contributing

Contributions are welcome! Please:

1. Fork the repository
2. Create a feature branch
3. Install development dependencies: `npm install`
4. Test your changes thoroughly: `npm test`
5. Submit a pull request

### Development Setup

This project uses aglint for filter list validation. To set up the development environment:

```bash
# Install aglint globally
npm install -g aglint

# Or install as a dev dependency
npm install

# Validate the filter list
npm run validate

# Run all tests
npm test
```

### Pre-commit Hook

A pre-commit hook is included that automatically validates filter list syntax before each commit. The hook will:

- Check if aglint is installed
- Validate all `.txt` files in the repository
- Prevent commits if syntax errors are found
- Provide helpful error messages

To skip validation (not recommended):

```bash
git commit --no-verify -m "your message"
```

### Adding New Platforms

To add support for a new social media platform:

1. Identify the main feed selectors using browser developer tools
2. Add blocking rules following the existing pattern
3. Add appropriate whitelist rules for important features
4. Test thoroughly before submitting

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by digital wellness and productivity tools
- Built on the excellent uBlock Origin platform
- Community contributions and feedback

## 📊 Impact

This filter list helps users:

- Reduce mindless scrolling
- Improve focus and productivity
- Maintain intentional social media use
- Preserve important communication features

## 🔄 Updates

The filter list is updated regularly to:

- Keep up with social media site changes
- Add support for new platforms
- Improve blocking effectiveness
- Fix false positives

---

**Remember**: This tool is designed to help you use social media more intentionally, not to completely eliminate it. The goal is to reduce mindless consumption while preserving useful features.
