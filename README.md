How the Website "WebCrypt" works    https://maximian3.github.io/WebCrypt-2025/

File Encryption:
The user uploads a file through the form on the website.
A password is entered for encryption.
The file is converted into a Base64 string (to handle the file data as text).
The website uses the CryptoJS library to encrypt the Base64 string using the AES (Advanced Encryption Standard) algorithm.
The encrypted output is saved as a new file with the .enc extension and downloaded by the user.

File Decryption:
The user uploads an encrypted file and provides the password.
The website decrypts the file using the same AES algorithm.
The decrypted data is converted back from Base64 to its original binary format.
The user can then download the restored file.

Encryption Details
Encryption Algorithm: AES (using a secret key derived from the password).

Process:
The password is transformed into an encryption key.
The file data is encrypted using AES, producing a secure text-based string.
The result is a protected .enc file that cannot be decrypted without the correct password.
File Extension: Encrypted files are saved with the .enc extension to indicate their protected status.

Advantages
Ease of Use: Users only need to upload a file and enter a password.
Local Processing: All encryption and decryption operations are performed locally in the browser, ensuring that no data is sent to a server, which enhances security.
