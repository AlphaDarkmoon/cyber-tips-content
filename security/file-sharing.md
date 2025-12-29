# Secure File Sharing

Learn how to share files safely while maintaining privacy and security.

## Secure Sharing Methods

### Cloud Storage Services
**Google Drive**
- Free: 15GB
- Sharing: Link or email access
- Security: Encryption at rest
- Features: Version history, collaboration

**Dropbox**
- Free: 2GB
- Sharing: Link with password option
- Security: 2FA support
- Features: File requests, smart sync

**OneDrive**
- Free: 5GB (Microsoft account)
- Sharing: Office integration
- Security: Personal vault
- Features: Real-time collaboration

**ProtonDrive**
- Privacy-focused
- End-to-end encryption
- Zero-access encryption
- Swiss privacy laws

### Encrypted File Transfer

**Temporary Sharing:**
- Firefox Send alternatives
- WeTransfer (2GB free)
- SendAnywhere
- Snapdrop (local network)

**Business Solutions:**
- Box
- ShareFile
- Tresorit (zero-knowledge)

## Email Attachment Security

### Best Practices
- Scan files with antivirus first
- Use ZIP encryption for sensitive files
- Send password separately
- Verify recipient before sending
- Avoid public email for confidential data

### File Size Limits
- Gmail: 25MB
- Outlook: 20MB
- Yahoo: 25MB
- **Solution:** Use cloud links instead

## Password Protecting Files

### ZIP Files (Windows/Mac)
```
Windows: 7-Zip with AES-256
macOS: Archive Utility with encryption
```

### PDF Files
- Adobe Acrobat: Document password
- Preview (Mac): Export with encryption
- Online tools: Use with caution

### Office Documents
- Word/Excel: File → Info → Protect Document
- Set opening password
- Enable read-only mode

## End-to-End Encrypted Sharing

**Tools:**
1. **Signal** - Encrypted messaging with file sharing
2. **Wire** - Business collaboration
3. **Tresorit** - Zero-knowledge cloud
4. **Sync.com** - Encrypted cloud storage
5. **SpiderOak** - No-knowledge privacy

## Link Sharing Security

### Secure Link Settings
- Set expiration date
- Require password
- Limit download count
- Disable resharing
- Track access logs

### What to Check
✓ Link is HTTPS  
✓ Password required  
✓ Expiration set  
✓ Recipient verified  
✓ Access logged  

## Business File Sharing

### Enterprise Solutions
- Microsoft SharePoint
- Google Workspace
- Box Business
- Citrix ShareFile

### Compliance Requirements
- HIPAA (healthcare)
- GDPR (EU data)
- SOC 2 certification
- ISO 27001 compliance

## Mobile File Sharing

### Secure Apps
- **AirDrop** (iPhone) - Encrypted, local
- **Nearby Share** (Android) - Bluetooth/WiFi
- **Snapdrop** - Browser-based, no install
- **Tresorit** - Encrypted mobile app

### Caution Areas
- Public Wi-Fi transfers
- Unknown recipients
- Large file sizes (use Wi-Fi)
- App permissions

## Version Control for Teams

**Git-based:**
- GitHub (public/private)
- GitLab (self-hosted option)
- Bitbucket

**Features:**
- Track changes
- Collaborate safely
- Roll back versions
- Access control

## Data Loss Prevention

### Before Sharing
1. **Classify data** - Public, internal, confidential
2. **Remove metadata** - Exif data, author info
3. **Scan for malware**
4. **Verify recipient**
5. **Use appropriate method**

### After Sharing
- Monitor access logs
- Revoke access if needed
- Delete expired shares
- Track downloads
- Audit regularly

## Metadata Removal

Files contain hidden information:
- Author name
- Company name
- Edit history
- GPS location (photos)
- Device information

**Tools to Remove:**
- ExifTool
- MAT2 (Linux)
- Adobe Acrobat (PDFs)
- Office "Inspect Document"

## Quick Decision Guide

**Public file, no security needed:**
→ Google Drive, Dropbox public link

**Sensitive file, trusted recipient:**
→ Cloud storage with password link

**Confidential business data:**
→ Enterprise solution with encryption

**Temporary share (1-time):**
→ Send, WeTransfer with expiration

**Maximum security:**
→ End-to-end encrypted service (Tresorit, ProtonDrive)

## Red Flags to Avoid

🚩 Unencrypted email for sensitive data  
🚩 Public links without passwords  
🚩 No expiration dates  
🚩 Unknown file sharing services  
🚩 HTTP (not HTTPS) uploads  
🚩 Suspicious file requests  

## Security Checklist

Before sharing files:
- ☐ Is this data sensitive?
- ☐ Is the recipient verified?
- ☐ Is the method secure?
- ☐ Is encryption needed?
- ☐ Should I set expiration?
- ☐ Have I removed metadata?
- ☐ Is password protection needed?
- ☐ Can I track access?

Remember: Once shared, you lose control. Choose your sharing method wisely!
