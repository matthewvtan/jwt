# JWT

To help prepare for API authentication tomorrow, research [JSON Web Tokens](https://jwt.io) (known as JWTs). This should take about 30 minutes. Answer the following questions and submit this README as your homework:

1. What are the 3 parts of a JWT?

    Header, Payload, Signature

2. What information does each part contain?

    Header: Type of token (JWT) & Hashing algorithm
    Payload: Claims (Reserved, Public, Private)
    Signature: Encoded Header + Encoded Payload + Secret Signed

3. Why do people use JWTs for authentication? A great resource to read would be https://jwt.io/introduction/.

    As JSON is less verbose than XML, when it is encoded its size is also smaller, making JWT more compact than SAML. This makes JWT a good choice to be passed in HTML and HTTP environments.

    Security-wise, SWT can only be symmetrically signed by a shared secret using the HMAC algorithm. However, JWT and SAML tokens can use a public/private key pair in the form of a X.509 certificate for signing. Signing XML with XML Digital Signature without introducing obscure security holes is very difficult when compared to the simplicity of signing JSON.
