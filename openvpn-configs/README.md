# Mecseki.net OpenVPN Configuration

## Setup Instructions

### For PIV/Smartcard Authentication:
1. Install OpenVPN client software (Not OpenVPN Connect!)
	This can be found at openvpn.net/community
2. Download configuration from this repository
3. Configure your PIV card
4. Update the PKCS#11 settings in the .ovpn file
5. Connect using your PIV card for authentication

### PKCS#11 Configuration:
See in the configuration.
On Windows, we are using the built in cryptoapicert, on linux, please get OpenSC.

## Security Notes
- Never share your private keys
- Keep your PIV card PIN secure
- Regularly update certificates before expiration
