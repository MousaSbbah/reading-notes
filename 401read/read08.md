## Review, Research, and Discussion

- **When is Basic Authorization used vs. Bearer Authorization?**

  - **Basic Authorization** : Provide a user name and password when making a request. In basic HTTP authentication
  - **Bearer Authorization** : Access to secure data by using JSON Web Token

- **What does the JSON Web Token package do?**
  Transfer information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

- **What considerations should we make when creating and storing a SECRET?**
  Must be private ,long and encoded

|                |                                                                                                                                                                                                            |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **encryption** | is the method by which information is converted into secret code that hides the information's true meaning.                                                                                                |
| **Token**      | Bearer Tokens are sent in the Authorization header of HTTP requests, just like with Basic and Digest Auth.                                                                                                 |
| **Bearer**     | The name “Bearer authentication” can be understood as “give access to the bearer of this token.                                                                                                            |
| **SECRET**     | is a mathematical computation applied to the payload of the JWT using a secret key. The purpose is to ensure that the message has not been altered and to recognize the signer to validate the JWT         |
| **JWT**        | JSON Web Token (JWT) a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. |

# Role-Based Access Control(RBAC)

**Role-based access control (RBAC)** is nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment. With tight adherence to access requirements established for each role, access management becomes much easier.
![RBAC](https://cdn.ttgtmedia.com/rms/onlineImages/itops-rbac.png)

## Benefits of RBAC

- Improving operational efficiency. With RBAC, companies can decrease the need for paperwork and password changes when they hire new employees or switch the roles of existing employees.
- Giving administrators increased visibility. RBAC gives network administrators and managers more visibility and oversight into the business, while also guaranteeing that authorized users and guests on the system are only given access to what they need to do their jobs.
- Reducing costs. By not allowing the user access to certain processes and applications, companies may conserve or more cost-effectively use resources, such as network bandwidth, memory, and storage.
- Decreasing risk of breaches and data leakage. Implementing RBAC means restricting access to sensitive information, thus reducing the potential for data breaches or data leakage.

![a](https://docs.confluent.io/platform/current/_images/rbac-overview.png)

## RBAC implementation (5 Stips)


1. **Inventory your systems**



2. **Analyze your workforce and create roles**



3. **Assign people to roles**



4. **Never make one-off changes**



5. **Audit**

![a](https://www.manageengine.com/device-control/images/RBAC3x.png)