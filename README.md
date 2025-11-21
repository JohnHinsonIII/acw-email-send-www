# ACW Email Campaign Manager

A complete email management solution with both SMTP (sending) and POP3 (receiving) capabilities, featuring a beautiful web interface for managing all your email communications.

## 📧 Overview

ACW Email Campaign Manager is a comprehensive dual-protocol email solution that allows you to:
- **Send** bulk email campaigns via SMTP
- **Receive** and manage emails via POP3  
- Manage recipient lists with ease
- View inbox with unread/read status
- Reply to received emails
- Track campaign progress in real-time
- Import/export recipient data via CSV

## ✨ Features

### SMTP - Email Sending
- **Bulk Email Sending**: Send personalized emails to multiple recipients
- **Recipient Management**: Add, edit, and organize recipients
- **CSV Import/Export**: Import recipient lists or export for backup
- **Test Email Mode**: Send test emails before full campaigns
- **Progress Tracking**: Real-time sending progress with visual indicators
- **Merge Tags**: Personalize emails with recipient data
- **HTML Support**: Rich HTML email content

### POP3 - Email Receiving
- **Inbox Management**: Fetch and view incoming emails
- **Unread Tracking**: Visual distinction between read and unread emails
- **Email Reader**: View full email content with sender, date, and body
- **Reply Function**: Quick reply to received emails
- **Delete Emails**: Remove unwanted messages
- **Stats Dashboard**: Total emails and unread count
- **Refresh/Check**: Manually fetch new emails from server

### User Interface
- **Dual Protocol Support**: Separate tabs for SMTP and POP3
- **Modern Design**: Clean, professional interface with gradient backgrounds
- **Responsive Layout**: Works on desktop, tablet, and mobile devices
- **Connection Status**: Monitor both SMTP and POP3 connections
- **Settings Panel**: Easy configuration for both protocols
- **Error Handling**: Clear error messages and feedback

## 🚀 Live Demo

**[Open Live Application](https://johnhinsoniii.github.io/acw-email-send-www/)** ← Try it now!

*Note: This is a frontend-only demo. Full email sending requires the backend server (see Backend Setup below).*

## 📦 What's Included

- `index.html` - Complete frontend application
- `INDEX.md` - Comprehensive documentation
- `README.md` - This file

## 🎯 Use Cases

### For Churches
- Send weekly bulletins and announcements
- Manage member communications
- Send event invitations and reminders
- Newsletter distribution

### For Organizations
- Marketing campaigns
- Newsletter distribution
- Event announcements
- Member communications

### For Businesses
- Customer newsletters
- Product announcements
- Promotional campaigns
- Transaction emails

## 🖥️ Technical Details

### Frontend Technologies
- **HTML5**: Semantic markup
- **CSS3**: Modern styling with gradients and animations
- **JavaScript**: Vanilla JS for interactivity
- **Responsive Design**: Mobile-first approach

### Backend Requirements (For Full Functionality)
- **Node.js**: v14 or higher
- **Express.js**: Web server framework
- **Nodemailer**: SMTP email sending
- **SMTP Server**: Gmail, SendGrid, or custom SMTP

## 📱 Interface Features

### Left Panel - Configuration
- **Connection Settings**: SMTP configuration
- **Email Details**: Subject, from address, reply-to
- **Recipient Management**: Add and manage email recipients
- **Import/Export**: CSV file handling

### Right Panel - Email Content
- **Rich Text Editor**: Create email content
- **Preview Mode**: See email before sending
- **Merge Tags**: Insert personalization tokens
- **Template Library**: Access sample templates

### Bottom Bar - Actions
- **Test Email**: Send to single recipient
- **Send Campaign**: Send to all recipients
- **Progress Tracking**: Real-time status updates
- **Error Reporting**: Detailed failure information

## 🎨 Design Highlights

### Color Scheme
- **Primary**: Deep blue (#2c5f7c) - Professional and trustworthy
- **Accent**: Gold (#d4af37) - Elegant and eye-catching
- **Background**: Purple gradient - Modern and engaging
- **Text**: Dark gray (#333) - Easy to read

### UI Components
- **Gradient Headers**: Eye-catching section headers
- **Card-based Layout**: Clean, organized sections
- **Smooth Transitions**: Polished animations
- **Status Indicators**: Visual feedback for all actions
- **Responsive Grid**: Adapts to all screen sizes

## ⚙️ Backend Setup (Optional)

For full email sending functionality, you need to set up the backend server:

### Quick Start
```bash
# 1. Install Node.js dependencies
npm install express nodemailer dotenv cors body-parser

# 2. Create .env file with SMTP settings
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your-email@gmail.com
SMTP_PASSWORD=your-app-password
RATE_LIMIT=10

# 3. Create server.js (contact for backend code)

# 4. Start server
node server.js

# 5. Open application
# Visit http://localhost:3000
```

### SMTP Configuration

#### Gmail Setup
1. Enable 2-Factor Authentication
2. Generate App Password
3. Use in SMTP settings:
   - Host: `smtp.gmail.com`
   - Port: `587`
   - User: Your Gmail address
   - Password: App Password (not regular password)

#### Other Providers
- **SendGrid**: Professional email service with API
- **Mailgun**: Developer-friendly email platform
- **Amazon SES**: Scalable cloud email service
- **Custom SMTP**: Any SMTP server you have access to

## 📊 Features Breakdown

### Recipient Management
```javascript
- Add recipients manually
- Import from CSV file
- Edit recipient information
- Delete recipients
- Export to CSV
- Bulk operations
```

### Email Composition
```javascript
- Subject line
- From address
- Reply-to address
- HTML email body
- Plain text fallback
- Merge tag support
- Preview functionality
```

### Campaign Sending
```javascript
- Test email mode
- Bulk sending
- Progress tracking
- Error handling
- Success reporting
- Rate limiting
- Retry logic
```

## 🔐 Security Considerations

### Best Practices
- ✅ Never store passwords in code
- ✅ Use environment variables for credentials
- ✅ Enable 2-Factor Authentication
- ✅ Use App Passwords (not regular passwords)
- ✅ Implement rate limiting
- ✅ Validate all input data
- ✅ Use HTTPS in production
- ✅ Sanitize HTML content

### Privacy & Compliance
- 📋 Obtain recipient consent
- 📋 Include unsubscribe links
- 📋 Honor unsubscribe requests
- 📋 Follow CAN-SPAM Act guidelines
- 📋 Implement data protection
- 📋 Maintain privacy policy

## 📈 Usage Tips

### Getting Started
1. Configure SMTP settings first
2. Test with your own email address
3. Start with small test campaigns
4. Monitor results carefully
5. Scale up gradually

### Best Practices
- **Personalization**: Use merge tags for names
- **Testing**: Always send test emails first
- **Timing**: Consider recipient time zones
- **Content**: Keep emails concise and clear
- **Subject Lines**: Make them compelling
- **Call to Action**: Include clear next steps
- **Mobile**: Test on mobile devices
- **Spam**: Avoid spam trigger words

### Rate Limiting
- Respect your SMTP provider's limits
- Gmail: ~500 emails per day (free)
- Professional services: Higher limits
- Use delays between sends
- Monitor for bounce backs

## 🛠️ Customization

### Easy Customizations
- Change color scheme in CSS
- Modify text and labels
- Adjust layout spacing
- Add your logo
- Custom email templates

### Advanced Customizations
- Add database integration
- Implement scheduling
- Add analytics tracking
- Create custom merge tags
- Build template library
- Add attachment support

## 📱 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers (iOS/Android)

## 📖 Additional Documentation

For complete documentation, see `INDEX.md` which includes:
- Quick Start Guide
- Architecture Overview
- File Reference
- Troubleshooting Guide
- Advanced Features
- Development Guide

## 🆘 Troubleshooting

### Common Issues

**Issue**: Emails not sending
- Check SMTP credentials
- Verify App Password (if using Gmail)
- Check firewall settings
- Test SMTP connection

**Issue**: Emails going to spam
- Use verified from address
- Include unsubscribe link
- Avoid spam trigger words
- Set up SPF/DKIM records

**Issue**: Connection errors
- Verify SMTP host and port
- Check internet connection
- Test with telnet
- Review firewall rules

## 🌟 Pro Features (Backend Required)

With backend server, you get:
- Real SMTP email sending
- Rate limiting and throttling
- Error retry logic
- Campaign history
- Email templates
- Scheduled sending
- Advanced analytics

## 📄 License

Free to use for personal and commercial projects.

## 🙏 Credits

Built for ACW (Association of Christian Writers) and church communication needs.

## 📞 Support

For questions or issues:
1. Check `INDEX.md` for detailed documentation
2. Review troubleshooting section
3. Test with simple configuration
4. Contact support if needed

## 🎓 Learning Resources

### Email Marketing
- [Email Marketing Best Practices](https://mailchimp.com/marketing-glossary/email-marketing/)
- [CAN-SPAM Act Compliance](https://www.ftc.gov/tips-advice/business-center/guidance/can-spam-act-compliance-guide-business)
- [HTML Email Design](https://www.campaignmonitor.com/dev-resources/guides/coding-html-emails/)

### Technical Resources
- [Node.js Documentation](https://nodejs.org/)
- [Nodemailer Guide](https://nodemailer.com/)
- [SMTP Setup](https://www.sparkpost.com/resources/email-explained/smtp-authentication/)

---

**Made with ❤️ for effective communication**

*Professional email campaigns made simple*
