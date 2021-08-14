# Read: Class 11 Authentication 

### What is OAuth

1. What is OAuth?
	- OAuth is an open-standard authorization protocol or framework that describes how unrelated servers
	 and services can safely allow authenticated access to their assets without actually sharing the initial, 
	related, single logon credential. In authentication parlance, this is known as secure, third-party, 
	user-agent, delegated authorization
	- from (https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

2. Give an example of what using OAuth would look like.
	- The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to 
	log on using another website’s/service’s logon. You then click on the button linked to the other website, the
	 other website authenticates you, and the website you were originally connecting to logs you on itself 
	afterward using permission gained from the second website.
	- from(https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)


3. How does OAuth work? What are the steps that it takes to authenticate the user?
	- Let’s assume a user has already signed into one website or service (OAuth only works using HTTPS). 
	The user then initiates a feature/transaction that needs to access another unrelated site or service. 
	The following happens (greatly simplified):

	- 1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
	- 2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
	- 3. The first site gives this token and secret to the initiating user’s client software.
	- 4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
	- 5. If not already authenticated to the authorization provider, the client may be asked to authenticate. 
	 After authentication, the client is asked to approve the authorization transaction to the second website.
	- 6. The user approves (or their software silently approves) a particular transaction type at the first website.
	- 7. The user is given an approved access token (notice it’s no longer a request token).
	- 8. The user gives the approved access token to the first website.
	- 9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
	- 10. The second website lets the first website access their site on behalf of the user.
	- 11. The user sees a successfully completed transaction occurring.
	- 12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact,
	 many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across
	 the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).
	- from(https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)


4. What is OpenID?
	-  OpenID is about authentication unlike OAuth that is about authorization
	- OpenID is for humans logging into machines


### Authorization and Authentication flows

1. What is the difference between authorization and authentication?
	- Authentication confirms that users are who they say they are. Authorization gives those users permission to access a resource.
	- from (https://www.okta.com/identity-101/authentication-vs-authorization/#:~:text=Authentication%20and%20authorization%20might%20sound,permission%20to%20access%20a%20resource.) 


2. What is Authorization Code Flow?
	- It's used to perform authentication and authorization in the majority of app types, 
	including single page apps, web apps, and natively installed apps
	- from (https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#:~:text=The%20OAuth%202.0%20authorization%20code%20flow%20is%20described%20in%20section,apps%2C%20and%20natively%20installed%20apps.)


3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
	-  OpenId Connect flow specifically designed to authenticate native or mobile application users
	- from (https://developers.onelogin.com/openid-connect/guides/auth-flow-pkce#:~:text=The%20Authorization%20Code%20Flow%20%2B%20PKCE,Proof%20Key%20for%20Code%20Exchange.)


4. What is Implicit Flow with Form Post?
	- uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. 
	 The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.
	- from (https://auth0.com/docs/flows/implicit-flow-with-form-post)


5. What is Client Credentials Flow?
	- it's a server to server flow


6. What is Device Authorization Flow?
	-  it's an OAuth 2.0 extension that enables devices with no browser or limited input capability to obtain an access token
	- from (https://oauth.net/2/device-flow/#:~:text=The%20OAuth%202.0%20Device%20Authorization,video%20to%20a%20YouTube%20channel.)


7. What is Resource Owner Password Flow?
	- flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token
	- from (https://www.oreilly.com/library/view/getting-started-with/9781449317843/ch04.html#:~:text=The%20Resource%20Owner%20Password%20Credentials,%2C%20optionally%2C%20a%20refresh%20token.&text=The%20primary%20difference%20is%20that,is%20accessible%20to%20the%20application.)

## Things I want to know more about
all of these are a bit too vague for me
i'd like to learn about OAuth more







