# Spring Boot and OAuth2

## There are several samples building on each other, adding new features at each step:

- simple: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties (if you visit the home page, you will be automatically redirected to GitHub).

- click: adds an explicit link that the user has to click to login.

- logout: adds a logout link as well for authenticated users.

- two-providers: adds a second login provider so the user can choose on the home page which one to use.

- custom-error: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.



## How to Add a Local User Database
- Many applications need to hold data about their users locally, even if authentication is delegated to an external provider. We don’t show the code here, but it is easy to do in two steps.

  - Choose a backend for your database, and set up some repositories (using Spring Data, say) for a custom User object that suits your needs and can be populated, fully or partially, from external authentication.

  - Implement and expose OAuth2UserService to call the Authorization Server as well as your database. Your implementation can delegate to the default implementation, which will do the heavy lifting of calling the Authorization Server. Your implementation should return something that extends your custom User object and implements OAuth2User.


## Adding an Error Page for Unauthenticated Users
- In this section, you’ll modify the two-providers app you built earlier to give some feedback to users that cannot authenticate. At the same time you’ll extend the authentication logic to include a rule that only allows users if they belong to a specific GitHub organization. The "organization" is a GitHub domain-specific concept, but similar rules could be devised for other providers. For example, with Google you might want to only authenticate users from a specific domain.

