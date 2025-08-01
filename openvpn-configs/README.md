# Mecseki.net OpenVPN Configuration

## Files
- `mecseki-vpn.ovpn`: OpenVPN client configuration
- `ca.crt`: Certificate Authority certificate

## Setup Instructions

### For PIV/Smartcard Authentication:
1. Install OpenVPN client software
2. Download both files from this repository
3. Configure your PIV card with PKCS#11 module
4. Update the PKCS#11 settings in the .ovpn file
5. Connect using your PIV card for authentication

### PKCS#11 Configuration:
Update the .ovpn file with your specific PIV module path and ID.

For Windows: Usually `C:\Program Files\...\your_piv_module.dll`
For Linux: Usually `/usr/lib/...your_piv_module.so`
For macOS: Usually `/usr/local/lib/...your_piv_module.dylib`

## Security Notes
- Never share your private keys
- Keep your PIV card PIN secure
- Regularly update certificates before expiration
