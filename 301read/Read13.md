# SENDING FORM DATA
![](https://i.stack.imgur.com/rKyZ1.png)
## The action attribute

In this example, the data is sent to an absolute URL — https://example.com:
```html
<form action="https://example.com">
```
Here, we use a relative URL — the data is sent to a different URL on the same origin:

```html
`<form action="/somewhere_else">`
```

# The method attribute

## The GET method
The GET method is the method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource." In this case, the browser sends an empty body. Because the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.

![](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/url-parameters.png)

The data is appended to the URL as a series of name/value pairs. After the URL web address has ended, we include a question mark (?) followed by the name/value pairs, each one separated by an ampersand (&). 

## The POST method

he POST method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.

![](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/network-monitor.png)





