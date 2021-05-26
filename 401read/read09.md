## Preview

1.  **Which 3 things had you heard about previously and now have better clarity on?**
    - MongoDB , Authorization/Authentication and Access control
1.  **Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**
    - More about Access control , O Auth and tests
1.  **What are you most excited about trying to implement or see how it works?**
    - Auth by using google and facebook


# O Auth

OAuth is an open-standard authorization protocol or framework that provides applications the ability for “secure designated access.” For example, you can tell Facebook that it’s OK for ESPN.com to access your profile or post updates to your timeline without having to give ESPN your Facebook password.

![OAuth](https://stormpath.com/wp-content/uploads/2016/04/what-is-oauth.jpg)

## How OAuth Works

- Step 1 – The User Shows Intent

- Step 2 – The Consumer Gets Permission

- Step 3 – The User Is Redirected to the Service Provider

- Step 4 – The User Gives Permission

- Step 5 – The Consumer Obtains an Access Token

- Step 6 – The Consumer Accesses the Protected Resource

![](https://docs.oracle.com/cd/E50612_01/doc.11122/oauth_guide/content/images/oauth/oauth_overview.png)

## OAuth and APIs


Developers build a lot of APIs. The API Economy is a common buzzword you might hear in boardrooms today. Companies need to protect their REST APIs in a way that allows many devices to access them. In the old days, you’d enter your username/password directory and the app would login directly as you. This gave rise to the delegated authorization problem.

**This is OAuth.**

![](https://d33wubrfki0l68.cloudfront.net/ecfd750086b8ac97fe5aaa08fdde917732b13225/f58f5/assets-jekyll/blog/oauth/biketoworkday-fb-login-f00e39aabbf3e44bc3570333643cbf5d966fc27367dbffd2623ff4a3694831c3.png)

OAuth is a delegated authorization framework for REST/APIs. It enables apps to obtain limited access (scopes) to a user’s data without giving away a user’s password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities. It supports server-to-server apps, browser-based apps, mobile/native apps, and consoles/TVs.


