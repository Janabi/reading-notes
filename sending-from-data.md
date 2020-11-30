# SENDING FORM DATA
Our main objectice is what exactly happened when the user press on the submit from data. **Where are the data going to be?** *What is the mechanism of this process?*

## Client/Server Architecture
So to make it easier to understand, the user will send a data on HTTP request to a server then the server will send it back at the same protocol (HTTP response).
![Figure1](https://developer.mozilla.org/files/4291/client-server.png)
At the end, as a user you will only see the stylish form (including HTML and CSS documents) but as we said previously this is exactly what is happening behind the sence in the back-end side.

## On the Client Side
The form element has two atrributes that are managed the transmission of data when the user press on the submit button.

- Action Attribute
This attribute determine where the data are going to send. These data will be sent as either relative or absolute URL.
```
<form action="https://google.com">
```
***OR***
```
<form action="/certain-route">
```
*If you leave the action empty, then the data will send on the same page.*

- Method Attribute
This attribute defines how the data is sent. There are two ways which they are 'GET' and 'POST'.
1. Get Method
This one is used by the browser to tell the server to send back the resource. The browser will send an empty body and these data instead will appended to the URL itself.
Lets take a look at this example and the figure of its result.
```
<form action="http://www.foo.com" method="GET">
  <div>
    <label for="say">What greeting do you want to say?</label>
    <input name="say" id="say" value="Hi">
  </div>
  <div>
    <label for="to">Who do you want to say it to?</label>
    <input name="to" id="to" value="Mom">
  </div>
  <div>
    <button>Send my greetings</button>
  </div>
</form>
```

![figure2](https://mdn.mozillademos.org/files/14685/url-parameters.png)

In this example, we saw that when the user will click on submit button. The data from these inputs (say and to) will append to the URL which they are going to be separated by ampersand and started with question mark.

2. POST Method
it is a different senario than GET method, which the browser uses to ask the server for a response that would provid data in the body of HTTP request. Then they will not append any data at the URL, instead they will appear in the body of HTTP request.
```
POST / HTTP/2.0
Host: foo.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 13

say=Hi&to=Mom
```

## Viewing HTTP Requests
* After submitting the form, the HTTP request will display if you are using "Google Chrome" got to inspect the following next steps:
1. Click the 'network' then the URL that you've been submitting for.
2. Then check at the bottom of header item where you will find the data displayed.

* Usually developers prefer POST above GET method because it will be insecure to put the passward on the URL and also there is a limit number of characters in the URL.