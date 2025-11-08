# Support

Need help with MetaPhotoAI? We're here to assist you!

## 📚 Documentation

Start with our comprehensive documentation:

- **Website:** [metaphotoai.io](https://metaphotoai.io)
- **User Guides:** [metaphotoai.io/docs](https://metaphotoai.io/docs)
- **Video Tutorials:** [metaphotoai.io/tutorials](https://metaphotoai.io/tutorials)
- **Blog & Tips:** [metaphotoai.io/blog](https://metaphotoai.io/blog)

## 💬 Get Help

### Email Support

For general questions, technical issues, or account help:

**hello@metaphotoai.io**

**Response time:** Within 24-48 hours on business days

Please include:
- Your MetaPhotoAI version (Help → About)
- Operating system and version
- Detailed description of the issue
- Steps to reproduce (if applicable)
- Screenshots (if helpful)

### Bug Reports

Found a bug? Please report it:

1. **GitHub Issues:** [Report a bug](https://github.com/rohaneh/metaphotoai-v3-releases/issues/new)
2. **Email:** hello@metaphotoai.io

When reporting a bug, please include:
- What you expected to happen
- What actually happened
- Steps to reproduce the issue
- App version and OS
- Any error messages
- Screenshots or screen recordings (if possible)

### Feature Requests

Have an idea for a new feature?

1. **GitHub Discussions:** [Suggest a feature](https://github.com/rohaneh/metaphotoai-v3-releases/discussions)
2. **Email:** hello@metaphotoai.io

Tell us:
- What feature you'd like to see
- Why it would be useful
- How you envision it working

## 🔍 Common Issues

### Installation Issues

#### macOS: "App can't be opened because it is from an unidentified developer"

**Solution:**
1. Right-click (or Control-click) the app
2. Select "Open" from the menu
3. Click "Open" in the dialog
4. The app will now open and be remembered

#### Windows: "Windows protected your PC"

**Solution:**
1. Click "More info"
2. Click "Run anyway"
3. The app will install normally

#### Linux: AppImage won't run

**Solution:**
```bash
chmod +x MetaPhotoAI-*.AppImage
./MetaPhotoAI-*.AppImage
```

### Login Issues

#### "Failed to sign in"

**Solutions:**
1. Check your internet connection
2. Verify your email/password
3. Try resetting your password
4. Clear browser cache (if using web)
5. Contact support if issue persists

#### "Device limit exceeded"

**Solution:**
- You've reached your plan's device limit
- Sign in to the app to see your active devices
- Deactivate an unused device
- Or upgrade your plan for more devices

### Metadata Generation Issues

#### "Out of credits"

**Solutions:**
1. Check your credit balance in the app
2. Wait for monthly renewal (subscription plans)
3. Purchase extra credits
4. Upgrade your subscription plan

#### "Failed to generate metadata"

**Solutions:**
1. Check your internet connection
2. Verify you're signed in
3. Try with a single image first
4. Check image file isn't corrupted
5. Try a different image format
6. Contact support if specific images fail

#### Generated metadata doesn't match expectations

**Solutions:**
1. Use Helper Text to provide context
2. Adjust settings (title length, keyword count, etc.)
3. Try adjusting the system prompt (advanced)
4. Use editorial mode for news/documentary images
5. Review and manually edit generated metadata

### Export Issues

#### EXIF writing fails

**Solutions:**
1. Ensure files aren't read-only
2. Close other apps using the images
3. Check file permissions
4. Try with JPEG (most compatible format)
5. Verify ExifTool is working (check logs)

#### FTP upload fails

**Solutions:**
1. Verify FTP credentials
2. Test connection in FTP settings
3. Try SFTP if FTP doesn't work
4. Check firewall settings
5. Verify remote server is accessible
6. Check file permissions on remote server

### Performance Issues

#### App is slow

**Solutions:**
1. Close unnecessary applications
2. Check available RAM (4GB minimum, 8GB recommended)
3. Reduce batch size (try smaller batches)
4. Clear app cache (Help → Clear Cache)
5. Update to latest version
6. Restart the app

#### Thumbnails not loading

**Solutions:**
1. Wait a moment (thumbnails generate in background)
2. Check available disk space
3. Verify image files exist and aren't corrupted
4. Restart the app
5. Clear thumbnail cache

### Update Issues

#### Updates not installing

**Solutions:**
1. Ensure you have admin/sudo permissions
2. Close all instances of the app
3. Try manually downloading the latest version
4. Check disk space
5. Temporarily disable antivirus (if blocking)

## 📊 System Requirements

Ensure your system meets the minimum requirements:

### macOS
- macOS 10.13 (High Sierra) or later
- 4 GB RAM (8 GB recommended)
- 500 MB free disk space

### Windows
- Windows 10 (64-bit) or Windows 11
- 4 GB RAM (8 GB recommended)
- 500 MB free disk space

### Linux
- 64-bit distribution (Ubuntu 18.04+, Fedora 32+)
- GLIBC 2.28 or later
- 4 GB RAM (8 GB recommended)
- 500 MB free disk space

## 🔧 Troubleshooting Tools

### Enable Debug Logging

To help diagnose issues:

1. Open the app
2. Go to Settings → Advanced
3. Enable "Debug Logging"
4. Reproduce the issue
5. Send logs to support

**Log locations:**
- **macOS:** `~/Library/Logs/MetaPhotoAI/`
- **Windows:** `%APPDATA%\MetaPhotoAI\logs\`
- **Linux:** `~/.config/MetaPhotoAI/logs/`

### Check Database

If data seems corrupted:

1. Find your database: `~/.metaphotoai-data/metadata.db`
2. Back it up first!
3. Check file size (shouldn't be 0 bytes)
4. Try opening with SQLite browser
5. Contact support if corrupted

### Reset Settings

If settings seem broken:

1. Close the app
2. Delete settings file:
   - macOS: `~/Library/Application Support/MetaPhotoAI/`
   - Windows: `%APPDATA%\MetaPhotoAI\`
   - Linux: `~/.config/MetaPhotoAI/`
3. Restart the app (creates fresh settings)

## 💰 Billing & Subscription

For billing questions:

- **Account Dashboard:** [metaphotoai.io/dashboard](https://metaphotoai.io/dashboard)
- **Email:** hello@metaphotoai.io

Common billing questions:
- Change subscription plan
- Cancel subscription
- Update payment method
- Request refund
- Download invoices

## 🎓 Learning Resources

### Getting Started
1. Install and sign in
2. Add your photo folders
3. Select images to process
4. Click "Generate Metadata"
5. Review and export

### Best Practices
- Use Helper Text for specialized content
- Adjust settings per folder for consistency
- Review AI-generated metadata
- Use templates for repeated workflows
- Leverage batch processing for efficiency

### Tips & Tricks
- Use color tags to organize images
- Set up folder-specific settings
- Create metadata templates
- Use keyboard shortcuts (CMD+SHIFT+M to generate)
- Filter images to find those needing metadata

## 📱 Stay Updated

- **Newsletter:** [Subscribe](https://metaphotoai.io/newsletter)
- **Blog:** [metaphotoai.io/blog](https://metaphotoai.io/blog)
- **Twitter:** [@metaphotoai](https://twitter.com/metaphotoai)

## 🤝 Community

Connect with other MetaPhotoAI users:

- **GitHub Discussions:** [Join discussions](https://github.com/rohaneh/metaphotoai-v3-releases/discussions)
- **User Community:** Coming soon!

## 📧 Contact

**General Support:** hello@metaphotoai.io
**Security Issues:** security@metaphotoai.io
**Billing Questions:** hello@metaphotoai.io

---

**We typically respond within 24-48 hours on business days.**

Thank you for using MetaPhotoAI! 🙏
