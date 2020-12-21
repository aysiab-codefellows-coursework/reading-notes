# Reading Assignment 08

### Review, Research & Discussion
> 1. When is Basic Authorization used vs. Bearer Authorization?
- Basic authentication uses user name aand a secret while bearer authentication uses a a token. 

> 2. What does JSON Web Token package do?
- JWTs are able to securely move data around as a JSON object.

> 3. What considerations should we make when creating and storing a SECRET?
- Security needs to be considered which is why SECRETs should be encrupted and kept away from public access. Consider keeping secrets as an environment variable.

### Definitions
**Encryption:** a algorithm used of converting information into a secret code
**Token:** more secure form of authentication than a password/secret
**Bearer:** a client that holds an authorized token
**Secret:** the digital code for a JSON Web Token known only by the client and application
**JSON Web Token:** a way to securely transmit information as a JSON object. A secret is used to help encrypt the information

