# Password Hashing and Security

## Hashing

Hashing is a process of converting data (in this case, a password) into a fixed-size string of characters, which is typically a hexadecimal or binary representation. This transformation is done by a hash function.

## Hash Function for Passwords

 A hash function takes a password and turns it into a unique jumble of characters, like a secret code. This code is stored in place of the actual password in a database. When you log in, the system takes your entered password, runs it through the same hash function, and checks if the resulting code matches the one stored in the database. If they match, you get access!

## Salting a Password

Salting a password means adding random data (called a "salt") to the password before hashing it. This adds complexity and makes it much harder for attackers to crack passwords using precomputed tables (rainbow tables) or common attack techniques.

## Finding the Salt

Hackers would need access to both the hashed password and the salt value to crack a salted password. The salt is typically stored alongside the hashed password in the database. So, if they breach the database and gain access to the password hashes, they would also have the salt values.

## bcrypt Overview

bcrypt is a popular password hashing algorithm that incorporates salting and multiple rounds of hashing to increase security. It's commonly used to store passwords securely in applications.

## Blowfish Block Cipher

The Blowfish block cipher used in bcrypt adapts to increased computation speeds by repeatedly applying the cipher in a loop, making it slower to calculate. This "key expansion" step requires more computational resources, which makes it resistant to brute-force attacks even on faster computers.

## Issues with Java Password Hashing

Two common password hashing issues in Java are:

1. **Java Password Hash**: This is not a recommended way to hash passwords as it often lacks key security features like salting and multiple rounds of hashing.

2. **Java Password Encryption**: Encryption is different from hashing and is not suitable for securely storing passwords. Encrypted passwords can potentially be decrypted if an attacker gains access to the encryption keys.

Always use secure and established password hashing libraries like bcrypt to store and verify passwords in Java applications.
