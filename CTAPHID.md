# CTAPHID API Commands

| Command Identifier | Parameters | Description |
| --- | --- | --- |
| Select | `aid: &[u8]` | Select the application |
| Calculate | `label: &'l [u8], hash: Option<Hash>, truncate: Option<bool>` | Calculate the authentication data for a credential given by label |
| CalculateAll | `challenge: &'l [u8], response: &'l [u8]` | Calculate the authentication data for all credentials |
| ClearPassword | None | Clear the password |
| Delete | `label: &'l [u8]` | Delete a credential |
| ListCredentials | `ListCredentials` | List all credentials |
| Register | `credential: Credential<'l>, overwrite: bool` | Register a new credential |
| Reset | None | Delete all credentials and rotate the salt |
| SetPassword | `kind: oath::Kind, algorithm: oath::Algorithm, key: &'l [u8], challenge: &'l [u8], response: &'l [u8]` | Set a password |
| Validate | `response: &'l [u8]` | Validate the password (both ways) |
| VerifyPin | `pin: &'l [u8]` | Verify PIN through the backend |
| SetPin | `new_pin: &'l [u8]` | Set PIN through the backend |
| ChangePin | `old_pin: &'l [u8], new_pin: &'l [u8]` | Change PIN through the backend |
| VerifyCode | `code: &'l [u8]` | Reverse HOTP validation |
| SendRemaining | None | Send remaining data in the buffer |
| GetCredential | `label: &'l [u8]` | Get Credential data |
| RenameCredential | `old_label: &'l [u8], new_label: &'l [u8]` | Rename Credential |
| YkSerial | None | Return serial number of the device. Yubikey-compatible command. Used in KeepassXC |
| YkGetStatus | None | Return application's status. Yubikey-compatible command. Used in KeepassXC |
| YkGetHmac

