# class_33

## JSON Web Token
### What is JSON Web Token
It defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

### where it usful?
Authorization

Information Exchange

What is the JSON Web Token structure?
a JWT typically looks like the following. Header.payload.Signature

JSON Web Tokens consist of three parts:

* 1. Header
The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.

* 2. payload
payload contains the claims. Claims are statements about an entity and additional data.

### types of claims:
* Registered claims: These are a set of predefined claims which are not mandatory but recommended, to provide a set of useful, interoperable claims. Some of them are: iss (issuer), exp (expiration time), sub (subject), aud (audience), and others.

* Public claims: These can be defined at will by those using JWTs. But to avoid collisions they should be defined in the IANA JSON Web Token Registry or be defined as a URI that contains a collision resistant namespace.

* Private claims: These are the custom claims created to share information between parties that agree on using them and are neither registered or public claims.

### How do JSON Web Tokens work?
In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.

Whenever the user wants to access a protected route or resource, the user agent should send the JWT, typically in the Authorization header using the Bearer schema.

note that with signed tokens, all the information contained within the token is exposed to users or other parties, even though they are unable to change it. This means you should not put secret information within the token.

### Why should we use JSON Web Tokens?
As JSON is less verbose than XML, when it is encoded its size is also smaller, making JWT more compact than SAML. This makes JWT a good choice to be passed in HTML and HTTP environments.
* Django Runserver Is Not Your Production Server
* A Production Stack
* A production setup usually consists of multiple components, each designed and built to be really good at one specific thing. They are fast, reliable and very focused.
* When a request arrives at your server, it should be passed to a dedicated web server
* The next component is an application server. It gets those fancy requests and uses them to construct Python objects which are usable by Django
