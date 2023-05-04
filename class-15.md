# Reading notes for class 15

## What is OAuth

**What is OAuth?**
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

**Give an example of what using OAuth would look like.**
The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

**How does OAuth work? What are the steps that it takes to authenticate the user?**
Step 1 – The User Shows Intent.
Step 2 – The Consumer Gets Permission.
Step 3 – The User Is Redirected to the Service Provider.
Step 4 – The User Gives Permission.
Step 5 – The Consumer Obtains an Access Token.
Step 6 – The Consumer Accesses the Protected Resource.

**What is OpenID?**
OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.

## Authorization and Authentication flows

**What is the difference between authorization and authentication?**
Authentication is the process of verifying who someone is, whereas authorization is the process of verifying what specific applications, files, and data a user has access to

**What is Authorization Code Flow?**
It enables a client application to obtain authorized access to protected resources like web APIs. The auth code flow requires a user-agent that supports redirection from the authorization server (the Microsoft identity platform) back to your application.So, it exchanges an Authorization Code for a token.

**What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**
During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).

**What is Implicit Flow with Form Post?**
As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets. While this is no longer considered a best practice for requesting Access Tokens, when used with Form Post response mode, it does offer a streamlined workflow if the application needs only an ID token to perform user authentication.

**What is Client Credentials Flow?**
A server to server flow that involves an application exchanging its application credentials, such as client ID and client secret, for an access token. This flow is best suited for Machine-to-Machine (M2M) applications, such as CLIs, daemons, or backend services, because the system must authenticate and authorize the application instead of a user.

**What is Device Authorization Flow?**
A polling protocol so errors served to the client must be expected prior to completion of user authentication. The user hasn't finished authenticating, but hasn't canceled the flow.

**What is Resource Owner Password Flow?**
An OAuth 2.0 extension that enables devices with no browser or limited input capability to obtain an access token. This is commonly seen on Apple TV apps.

## Things I want to know more about

Just authentication in general and how it works along with all the flows.
