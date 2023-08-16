# CTAPHID API Commands

| Command Identifier | Parameters | Description |
| --- | --- | --- |
| Select | `aid: &[u8]` | Select the application |
| Calculate | `Calculate<'l>` | Calculate the authentication data for a credential given by label |
| CalculateAll | `CalculateAll<'l>` | Calculate the authentication data for all credentials |
| ClearPassword | None | Clear the password |
| Delete | `Delete<'l>` | Delete a credential |
| ListCredentials | `ListCredentials` | List all credentials |
| Register | `Register<'l>` | Register a new credential |
| Reset | None | Delete all credentials and rotate the salt |
| SetPassword | `SetPassword<'l>` | Set a password |
| Validate | `Validate<'l>` | Validate the password (both ways) |
| VerifyPin | `VerifyPin<'l>` | Verify PIN through the backend |
| SetPin | `SetPin<'l>` | Set PIN through the backend |
| ChangePin | `ChangePin<'l>` | Change PIN through the backend |
| VerifyCode | `VerifyCode<'l>` | Reverse HOTP validation |
| SendRemaining | None | Send remaining data in the buffer |
| GetCredential | `GetCredential<'l>` | Get Credential data |
| RenameCredential | `RenameCredential<'l>` | Rename Credential |
| YkSerial | None | Return serial number of the device. Yubikey-compatible command. Used in KeepassXC |
| YkGetStatus | None | Return application's status. Yubikey-compatible command. Used in KeepassXC |
| YkGetHmac

