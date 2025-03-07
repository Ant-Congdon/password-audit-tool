# Online Account Security Audit Tool

## Overview
A standalone web-based security audit tool designed to help users assess the security of their online accounts. This tool runs entirely in the browser, prioritizing privacy and security while providing valuable password breach detection capabilities.

## Key Features
- **Client-Side Operation**: Runs completely in-browser with no server requirements
- **Password Security Check**: Integrates with HaveIBeenPwned (HIBP) using k-anonymity protocol
- **Secure Password Handling**: 
  - SHA-1 hashing implementation
  - Only displays last 5 characters of hashes
  - No password storage or transmission
- **Security Audit Features**:
  - Multi-Factor Authentication (MFA) tracking
  - Privacy settings assessment
  - Security recovery settings review
  - Identity linkage documentation

## Security Measures
- Content Security Policy (CSP) implementation
- No external dependencies (except HIBP API)
- Data sanitization on all inputs
- Automatic data clearing on page close/refresh
- OWASP Top 10 compliant

## Usage
1. Open `index.html` in a modern web browser
2. Input account details in the provided form
3. Passwords are automatically hashed and checked against HIBP
4. Export or print results as needed

## Export Options
- Print to PDF
- Save as HTML
- All sensitive data is appropriately masked in exports

## Technical Requirements
- Modern web browser with JavaScript enabled
- Internet connection (for HIBP API checks)
- No additional software required

## Privacy Considerations
- No data storage
- No cookies or local storage used
- No analytics or tracking
- Only first 5 characters of password hashes sent to HIBP

## Development
To modify or enhance the tool:
1. Clone the repository
2. Modify the single HTML file as needed
3. Test thoroughly in various browsers
4. Ensure CSP compliance for any new features

## Testing
Recommended testing procedures:
- Cross-browser testing
- Privacy mode testing
- Offline capability testing
- Export function verification

## Known Limitations
- Requires internet connection for HIBP checks
- Single-page application (no data persistence)
- Limited to browser security constraints

## Contributing
Contributions welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request
4. Ensure all security measures remain intact


## License
GNU 3.0

## Version History
- v1.0.0 - Initial release
  - Basic functionality
  - HIBP integration
  - Export capabilities

## Acknowledgments
- HIBP API service
- Security best practices from OWASP

---
Note: This tool is designed for educational and personal audit purposes. Always follow your organization's security policies and procedures.
