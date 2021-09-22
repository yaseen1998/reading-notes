# class-14
## What is OAuth?

OAuth is a framework that allows websites and services to share assets among users. It provides secure, third-party, user-agent, delegated authorization. OAuth open-standard authorization protocol/framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing initial credentials.

Authentication is the process of a user/subject proving its ownership of a presented identity, by providing a password or some other uniquely owned or presented factor. Simply: it is the process of verifying who a user is.

Authorization is the process of letting a subject access resources after a successful authentication. Simply: it is the process of verifying what they have access to.

OAuth (Open AUTHorization) is about authorization in particular and not directly about authentication.

Most OAuth scenarios represent two unrelated sites or services trying to accomplish something on behalf of users or their software. The three have to work together involving multiple approvals for the completed transaction to get authorized. An example is when you try to log into a website and it offers one or more opportunities to log in using another website or service, for example, signing into instagram using your facebook account.

## Give an example of what using OAuth would look like.
The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

## How does OAuth work? What are the steps that it takes to authenticate the user?
oAuth doesn’t share password data but instead uses authorization tokens to prove an identity between consumers and service providers

## What is OpenID?
 OpenID is about authentication: as a commenter on StackOverflow pithily put it: "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."
 
 ## Authorization and Authentication flows
 
 ### What is the difference between authorization and authentication?
Authentication is the process of a user/subject proving its ownership of a presented identity, by providing a password or some other uniquely owned or presented factor. Simply: it is the process of verifying who a user is.

Authorization is the process of letting a subject access resources after a successful authentication. Simply: it is the process of verifying what they have access to.

### What is Authorization Code Flow?
Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow (defined in OAuth 2.0 RFC 6749, section 4.1), which exchanges an Authorization Code for a token. Your app must be server-side because during this exchange, you must also pass along your application's Client Secret, which must always be kept secure, and you will have to store it in your client.

### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).

### What is Implicit Flow with Form Post?
Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls. With this method, you don’t need to obtain, maintain, use, and protect a secret in your application.

### What is Client Credentials Flow?
With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow (defined in OAuth 2.0 RFC 6749, section 4.4), in which they pass along their Client ID and Client Secret to authenticate themselves and get a token.

### What is Device Authorization Flow?
With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (ratified in OAuth 2.0), in which they pass along their Client ID to initiate the authorization process and get a token.

### What is Resource Owner Password Flow?
Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.

