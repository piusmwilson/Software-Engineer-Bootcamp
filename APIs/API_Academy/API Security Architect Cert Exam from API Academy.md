# API Security Architect Exam Answers – API Academy

## Question 1: Match the examples of threat models that correspond with the OAuth 2.0 components:

- **Client Threats ->** _Attackers obtaining client secrets. Attackers phishing for credentials using compromised or embedded browser. Open redirection on the client side._
- **Endpoint Threats ->** _Phishing by counterfeit authorization server. Interception of traffic to resource server._
- **Token Threat –>** _Token theft. Disclosure of client credentials during token transmission. Obtaining client secrets from either the database or through guesswork._


## Question 2: When a token is stolen, it makes the system vulnerable to:

- Certificate pinning
- Cross-site scripting and denial of service attacks
- Attackers phishing for credentials using a compromised or embedded browser
- **_Man-in-the-middle and man-in-the-browser attacks_**


## Question 3: Match the following token types with the correct statements:

- **ID Token ->** _…contains claims about authentication status of an end user, and indicates the status of the authentication._
- **Access Token ->** _….indicates the status of authorization. It can be used by a client to retrieve additional user information, but is not intended to carry information about the user._
- **Refresh Token ->** _…is used to get a new access token once the previous token has expired._
- **JSON Web Token ->** _…is a signed and/or encrypted, stateless and self-contained token format, carrying all the necessary information within their header, payload, and signature._

## Question 4: In an OAuth 2.0 Authorization flow, where Joe is the resource owner who wants to use a third-party application to access his banking information, sort the following steps in the flow in the order they will be happening:

- **_Joe logs into a third-party application and wishes to access his banking information from the application._**
- **_The third-party application sends an authorization request to the bank’s authorization server. It redirects Joe’s browser to the login screen of the authorization server._**
- **_The authorization server asks Joe to authorize the third-party application’s access to his banking information._**
- **_Joe grants or denies the third-party application’s access to the banking information._**

## Question 5: Match the following statements:

- **The OAuth 2.0 protocol… ->** _…excels at delegated authorization._
- **Scope, a mechanism in OAuth 2.0… ->** _…is designed to limit an application’s access to a resource such as user’s data._
- **The client ID… ->** _…is a public identifier for apps and is typically encoded in a multi-character hex string._
- **The authorization code… ->** _…is not enough for the client application to fetch the requested resources from the resource server and is subsequently exchanged for an access token._

## Question 6: One consideration to mitigate client threats is through Application Access Control. The principles of application access control are (select all that apply):

- **_Establish credentials with a handshake or registration during client installation, instead of hosting the secrets in code._**
- **_Consistently implement monitoring and detection_**
- **_Move the credentials to a server_**
- Do NOT move the credentials to a server

## Question 7: One of the threats to the authorization server involves redirection hijack. Which statement about redirection hijack is true?

- A good consideration to address redirect hijack is to implement a proof key for code exchange (PKCE).
- The redirection hijack happens once authorization has been granted with either an authorization code or implicit grant type. Instead of redirecting back to the client, the authorization server is fooled into redirecting to somewhere other than the client.
- **_All options are correct_**
- One way to mitigate the risk of redirection hijack is to whitelist the redirect URIs on the authorization server.

## Question 8: Which of the following is part of JWT best practices?

- Using claims to the fullest extent
- Setting a shorter timeout
- Never letting the header alone drive verification
- **_All options are correct_**

## Question 9: Which of these characteristics is an advantage of JSON Web Tokens? (Select all that apply)

- JWT is checked against the token registry on the authorization server.
- **_JWT is stateless._**
- JWT is stateful.
- **_As a versatile token format, JWT’s usage spans across the OAuth 2.0 and OpenID Connect workflow: It can be used as a format for ID tokens, access tokens, and refresh tokens._**
- **_JWT is programming language-agnostic._**

## Question 10: Match the following statements:

- **TLS (Transport Layer Security) and SSL (Secure Sockets Layer)… ->** _…are cryptographic protocols that help you keep the internet connection and transfer of data secure._
- **Rate limiting, Message validation, Encryption and signing and Access control… ->** _…are standard security functions from the API gateway world that are important when it comes to protecting the APIs and mitigating API threats._
- **HTTP access control… ->** _…provides an access authentication feature and allows servers to challenge clients and reject unauthorized access._
- **TLS trust attacks… ->** _…can be divided into three categories – certificate authority vulnerabilities, human vulnerabilities and man in the middle issues._

## Question 11: Evaluate the following statement. With stateless tokens becoming more widely adopted, OAuth 2.0 is increasingly relying on security embedded within the token itself. While TLS provides an extra layer of security, token theft is still possible.

- False
- **_True_**

## Question 12: Which statement about OAuth 2.0 is correct? (Select all that apply)

- The OAuth 2.0 core framework has not really been evolving as contributors are not allowed to publish additional specifications.
- **_OAuth 2.0 has a reputation to be complicated and difficult to implement, not only because of the various grant types but also because the specification itself is less prescriptive._**
- OAuth 2.0 authentication was designed to address vulnerabilities in OpenID Connect authorization protocol.
- **_Like other open-source frameworks of similar scale and magnitude, a long list of RFC specifications makes OAuth 2.0 potentially overwhelming._**

## Question 13: Evaluate the following statement. APIs give client-side developers (and potential hackers) much more finely-grained access into the backend than a typical website or application does.

- **_True_**
- False

## Question 14: Which statement about APIs is correct? (Select all that apply)

- **_For APIs, we CANNOT rely on the same security methods and technologies that we use to secure the browser-centric web applications._**
- **_APIs are fundamentally different from the traditional browser-centric web and therefore have a unique risk profile._**
- APIs DO NOT share any underlying technologies with traditional browser-centric web applications.
- **_Well-designed APIs are, by nature, more transparent than websites and therefore more vulnerable._**

## Question 15: Evaluate the following statement. The UserInfo endpoint is an OAuth 2.0 protected resource that lives in the authorization server.

- False
- **_True_**

## Question 16: It is an extension of OAuth 2.0 and works not only to eliminate OAuth 2.0 vulnerabilities, but also to fill authentication gaps within OAuth 2.0, such as better enabling SSO. Within the authorization flow, an additional ID token acts as an encrypted fingerprint that travels through the flow with the access token. At the API endpoint, it can be decoded to reveal user information for identity verification. What is being described?

- HTTP Access Control
- TLS / SSL protocol
- **_OpenID Connect protocol_**
- Implicit grant type

## Question 17: Which statement about OpenID Connect is correct?

- The ID Token acts like an encrypted fingerprint that travels through the flow with the access token.
- Within the Authorization flow, if “openid” is included as the scope, an additional ID Token is generated along with the Access Token.
- **_All options are correct_**
- The OpenID Connect protocol is an extension of OAuth 2.0 that is filling in the authentication gaps within OAuth 2.0, such as better enabling SSO.

## Question 18: The industry standard authorization protocol that permits a user to grant an application access to a protected resource without exposing the user’s password credentials is called:

- **_OAuth 2.0_**
- OpenID 2.0
- OpenID Connect
- Access Token

## Question 19: POODLE, BEAST, CRIME, BREACH, and HEARTBLEED are:

- Cryptographic protocols that help you keep the internet connection and transfer of data secure
- Authorization and authentication features
- The most typical components in the API security domain
- **_Historical vulnerabilities related to TLS/SSL protocols_**

## Question 20: Evaluate the following statement. OAuth 2.0 alone as a framework is no longer sufficient, and this is why OpenID Connect has become more relevant than ever before, as it offers a standardized and prescriptive method for delegated authentication.

- False
- **_True_**

## Question 21: Which statement about JSON Web Tokens is correct? (Select all that apply)

- **_Every JSON Web Token comprises three elements – header, payload and signature._**
- JWT is NOT part of the Javascript Object Signing and Encryption framework.
- **_JWT is a token format, an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object._**
- Higher verbosity is a characteristic that encourages usage of JWT tokens.

## Question 22: Evaluate the following statement. As long as your API is considered private and only used by your direct applications, you do not need to add extra security because no one will be aware of your API.

- **_False_**
- True

## Question 23: In a stateless token scenario, sort the following steps in the order they will be happening. After the client starts the OAuth 2.0 authorization process…

- **_The authorization server validates the client’s request and generates a JWT (which it encrypts and signs using a private key)._**
- **_The authorization server returns the JWT to the client._**
- **_The client makes a request to the resource server with the JWT and the server must validate the token with its private key._**
- **_The server’s protected routes will check for a valid JWT in the Authorization header, and if it is present, the client will be allowed to access protected resources._**

## Question 24: Evaluate the following definition. This implementation can help address the threat of redirect hijacks. In this implementation, the client generates a hashed secret and hashing method and sends them to the authorization server on code request. The secret is then used by the authorization server to verify a subsequent token request. As it requires both the client and server to participate, it helps address vulnerabilities, particularly in mobile apps.

- URL redirect
- **_A proof key for code exchange (PKCE)_**
- Cross-Origin Resource Sharing (CORS)
- Access and refresh tokens

## Question 25: Match the authorization grant types supported by OAuth 2.0 with the correct statement:

- **Authorization code ->** _The resource owner’s credentials are never shared with the client application and the resource server. The access token is never shared with the resource owner. It is the most secure and most common grant type today._
- **Implicit ->** _The client is issued an access token directly. No intermediate credentials (such as an authorization code) are issued. The authorization server does not authenticate the client._
- **Resource owner password credentials ->** _This grant type should only be used when there is a high degree of trust between the resource owner and the client, such as if the resource owner is the sole owner or operator of the device. Given the nature of this grant type, the ability of a person to impersonate the resource owner is highly likely, making it incredibly easy for hackers to have complete access. Use this type only when other authorization grant types are not available._
- **Client credentials ->** _This grant type is typically used when the client is acting on its own behalf or is requesting access based on a previously arranged authorization. Example use cases are typically for non-interactive applications such as a Command Line Interface, a daemon, or any service running in a backend server that doesn’t require any interaction with the end user. Many IoT devices also fall into this category. In all these examples, the client application would request and receive the access token without the user having any access to the protected resources._