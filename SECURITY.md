# Security Policy

## Supported Versions

We actively support the following versions of MetaPhotoAI with security updates:

| Version | Supported          |
| ------- | ------------------ |
| 3.0.x   | :white_check_mark: |
| < 3.0   | :x:                |

We recommend always using the latest version to ensure you have the most recent security updates.

## Reporting a Vulnerability

We take security seriously at MetaPhotoAI. If you discover a security vulnerability, please help us protect our users by reporting it responsibly.

### How to Report

**DO NOT** create a public GitHub issue for security vulnerabilities.

Instead, please email us directly at:

**security@metaphotoai.io**

Please include:

1. **Description** - A clear description of the vulnerability
2. **Steps to Reproduce** - Detailed steps to reproduce the issue
3. **Impact** - Your assessment of the potential impact
4. **Affected Versions** - Which versions are affected (if known)
5. **Suggested Fix** - Any suggestions for fixing the issue (optional)

### What to Expect

1. **Acknowledgment** - We'll acknowledge receipt within 48 hours
2. **Investigation** - We'll investigate and validate the report
3. **Updates** - We'll keep you informed of our progress
4. **Resolution** - We'll work on a fix and release it as soon as possible
5. **Credit** - With your permission, we'll credit you in the release notes

### Security Update Process

1. We develop and test a fix privately
2. We release a security update
3. We publish a security advisory (if appropriate)
4. We notify affected users via the app

## Security Best Practices

As a user, you can help keep your data secure:

### Account Security

- ✅ Use a strong, unique password for your MetaPhotoAI account
- ✅ Enable two-factor authentication (if available)
- ✅ Don't share your account credentials
- ✅ Log out on shared computers

### Data Protection

- ✅ Keep your operating system updated
- ✅ Use antivirus software
- ✅ Keep MetaPhotoAI updated to the latest version
- ✅ Be cautious about who has physical access to your computer
- ✅ Regularly back up your metadata database

### Network Security

- ✅ Use secure networks (avoid public Wi-Fi for sensitive operations)
- ✅ Use SFTP instead of FTP when possible for uploads
- ✅ Verify SSL certificates when using the web dashboard

### FTP/SFTP Credentials

- ✅ MetaPhotoAI encrypts your FTP credentials using OS-level encryption
- ✅ Credentials are stored locally, never sent to our servers
- ✅ Use strong passwords for your FTP accounts
- ✅ Regularly rotate FTP passwords

## Security Features

MetaPhotoAI includes several security features:

### Encryption

- **OS-Level Encryption** - Sensitive data (auth tokens, FTP credentials, device IDs) encrypted using your operating system's keychain/credential manager
- **HTTPS** - All communication with our servers uses HTTPS
- **Secure Storage** - Local database stored on your machine with encryption for sensitive fields

### Authentication

- **OAuth 2.0** - Industry-standard authentication via Clerk
- **Session Management** - Automatic session expiration
- **Device Activation** - Prevents unauthorized device usage

### Data Privacy

- **Local Processing** - Your images are processed locally when possible
- **Temporary Storage** - Images sent to AI are temporarily processed and never permanently stored
- **Data Control** - You control your data - export or delete anytime

### Code Signing

- **macOS** - App is signed and notarized by Apple
- **Windows** - App is code-signed with a valid certificate
- **Integrity** - Ensures the app hasn't been tampered with

## Known Security Considerations

### Image Processing

When generating metadata:
- Images are converted to base64 and sent to our backend
- Images are temporarily processed by AI models (OpenRouter)
- Images are automatically deleted after 30 days
- Thumbnails (not full images) are retained for audit purposes

### Network Access

The app requires internet access for:
- Authentication (Clerk)
- Metadata generation (Convex + OpenRouter)
- Auto-updates (GitHub Releases)
- Notification polling

The app does NOT:
- Access your images without permission
- Upload your images to permanent storage
- Share your data with third parties (except AI processing)
- Run background processes without your knowledge

## Third-Party Services

MetaPhotoAI integrates with:

- **Clerk** - Authentication ([security](https://clerk.com/security))
- **Convex** - Backend ([security](https://www.convex.dev/security))
- **OpenRouter** - AI processing ([privacy](https://openrouter.ai/privacy))
- **GitHub** - Auto-updates (Microsoft-owned)

Each service has its own security practices and policies.

## Compliance

MetaPhotoAI is designed with privacy in mind:

- No permanent storage of your images
- Local metadata storage
- Secure credential management
- Transparent data handling

## Questions?

For security-related questions that aren't vulnerabilities, please email:

**hello@metaphotoai.io**

---

Last updated: January 2025
