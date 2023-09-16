# Authentication and Authorization

## What does it mean to authenticate a user?

To identify the user based on some credits he provides and he only knows such as a password and a username or email.

## What does it mean to authorize a user?

To let the user having more accessabilty and control over the system than the normal user.

## What are the three possible outcomes of the AuthenticationManager’s authenticate() method?

- An `AuthenticationManager` can do one of 3 things in its authenticate() method:
  - Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.
  - Throw an AuthenticationException if it believes that the input represents an invalid principal.
  - Return null if it cannot decide.

## Spring Auth cheat sheet

1. Step 1: set up a user model and repo
2. Step 2: create a controller for that model
3. Step 3: UserDetailsServiceImpl implements UserDetailsService
4. Step 4: ApplicationUser implements UserDetails
5. Step 5: WebSecurityConfig extends WebSecurityConfigurerAdapter
6. Step 6: registration page
7. Step 7: login page
