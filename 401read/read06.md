## Review, Research, and Discussion

- **Explain what a “Singleton” is (in Computer Science terms)**
  Singleton is object that can have only a single, unique instance, with a single point of access.

- **Explain how the Singleton pattern can be used with Node modules, specifically with classes**
  Node.js module system provides simple way to implement Singleton using `module.exports`. Module will be cached when it is accessed using `require()` statement. So our module is merely a **cached** instance although it behaves like a **Singleton**.

- **If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?**
  I will start with build the Classes with methods that i needed and export these classes by using `module.exports`

|                                 |                                                                                                                                                                                                                                    |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Router Middleware**           | Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of `express.Router()`.                                                                                            |
| **Dynamic Module Loading**      | allows you to dynamically load modules only when they are needed, rather than having to load everything up front.                                                                                                                  |
| **Singleton Pattern**           | Singleton is object that can have only a single, unique instance, with a single point of access.                                                                                                                                   |
| **CRUD -> REST Method Matches** | (create-->post) ,(read-->get) ,(update-->put) ,(delete-->delete)                                                                                                                                                                   |
| **Mock Testing**                | Mocking is a process used in unit testing when the unit being tested has external dependencies. The purpose of mocking is to isolate and focus on the code being tested and not on the behavior or state of external dependencies. |

# Authentication

**Definition**: Authentication is the process of recognizing a user’s identity. It is the mechanism of associating an incoming request with a set of identifying credentials. The credentials provided are compared to those on a file in a database of the authorized user’s information on a local operating system or within an authentication server.

## Basic Authentication

**How does it work?**

- Get the username and password from user
- Encode it using base64 algorithm
- Set it in the Authorization header and send it along each HTTP Request.
  ![](https://d33wubrfki0l68.cloudfront.net/058bd56d158c5de6cd41b0f15adf9b08a5a9e26c/b02eb/media/auth_systems/basic.png)

**Advantages**

- Easy and simple to implement
- APIs are faster since there is no complex encryption/decryption involved

**Disadvantages**

- Basic Auth implemented in a non-SSL (HTTPS) network is a huge security vulnerability .It is easy to decode an Base64.
- Sending passwords over all the HTTP request provides a pool of requests for attackers to pick passwords from. Once they crack one the system becomes open for attacks.

## Securing Passwords with `Bcrypt` Hashing Function
![](https://cdn.lynda.com/course/2813266/2813266-637490915727128526-16x9.jpg)
**bcrypt** is a password-hashing function , Besides incorporating a salt to protect against rainbow table attacks, bcrypt is an adaptive function: over time, the iteration count can be increased to make it slower, so it remains resistant to brute-force search attacks even with increasing computation power.

**Install via NPM**

```
npm install bcrypt
```

**Hash Info**
![](https://i.imgur.com/al3kptj.jpg)
The characters that comprise the resultant hash are .
`ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789$`

Resultant hashes will be 60 characters long and they will include the salt among other parameters, as follows:

`$[algorithm]$[cost]$[salt][hash]`

- 2 chars hash algorithm identifier prefix. `"$2a$" or "$2b$"` indicates BCrypt
- Cost-factor (n). Represents the exponent used to determine how many iterations 2^n
- 16-byte (128-bit) salt, base64 encoded to 22 characters
- 24-byte (192-bit) hash, base64 encoded to 31 characters
