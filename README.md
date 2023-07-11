# DSA_cipher

# Cipher for Electronic signature  
#Python #PyQT  
  
University project from the subject "Cryptology".  
Author of the assignment: Petr Žáček; Tomas Bata University in Zlín; Faculty of Applied Informatics (Software Engineering). 2021  
Rating: 100%  

## Official assignment  
(Translated from Czech, edited)

Your final project involves developing an application to facilitate electronic file signing. The underlying principle of electronic signatures is depicted in the figure below.  
  
The SHA-256 hash function can be used for signing virtually any file type and size (files should be loaded with "rb"). Your solution will incorporate the following features:  

- Loading files for signature (using fileDialog).
- Displaying detailed information about the file to be signed, including the name, path, file type (extension), size, modification date, etc.
- Signing the file using the RSA and SHA3-512 Keccak functions, which were implemented in the previous task.
- Verifying the signature.
- Generating a key pair with the capability to export to files with .priv and .pub extensions.
- The user interface should be fully interactive, including file selection in a dialog box (fileDialog), and buttons. There should be minimal to no requirement for text input fields.
  
#### Additional Information:  
- The electronic signature (output after hashing and RSA encryption) will be saved as a .sign file. The content of the file will follow this format: RSA_SHA3-512 SIGN_V_BASE64. For example, "RSA_SHA3-512 QWhvaiBQZXBvLCBqYWsgc2UgbcOhxaEgPw==".
- The .sign file will be bundled with the signed document into a .zip file, which the user can then export to any desired location (using fileDialog).
- The key pair will consist of two files, one with a .priv suffix (private key) and the other with a .pub suffix (public key). The contents of these files will be in the form: RSA PRIVATE_KEY_IN_BASE64 and RSA PUBLIC_KEY_IN_BASE64.
-  Authentication should take place when the public key and the .zip file are selected. Manual unzipping of the signature should not be necessary.
  
#### Scoring Criteria:
- Loading the file for signing and displaying basic information (name, path, creation date, type, etc.): 2 points
- Generating keys and signing the file using SHA3-512 and RSA: 4 points
- Verifying a document based on an electronic signature: 4 points
- Managing files with keys and electronic signatures (loading and saving files with .priv, .pub, and .sign extensions (.zip)): 4 points
- GUI (fully interactive with buttons for loading/saving files, displaying necessary information): 4 points
- Artistic impression: 2 points
- Bonus points are available for creativity.
