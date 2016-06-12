# AdvanceJSLogging

## Introduction

Console object provides access to browser's debugging console. we all have used javascript to send messages but we can use it to do more than just send messages. 

## Javascript Log Levels

There are 5 core logging level method on the console object . The advantage of using log level is that it helps the fellow developer to  the message. Also, you can use it communicate with other by providing additional information. For eg. if you sending message through console.error, you are informing that there is something wrong so that one can step and debug what went wrong. Apart from this we can filter different kind of messages in the browser so that messages comes in handy to read.

### Warn 
Sends message to the console window, prefaced by a warning symbol. Objects that are passed by using the command are converted to a string value.
 
 `console.warn("This is warning message!");` 
 
 ![Image of Warning Console ](https://github.com/dipikam86/AdvanceJSLogging/blob/master/images/warn.png)
 
### Info
Sends message to the console window. The message is prefaced by an information symbol.
 
 `console.info("This is info !");` 
 
 ### Debug
Sends message to the console window, prefaced by a warning symbol. Objects that are passed by using the command are converted to a string value.
 
 `console.debug("This is debug !");` 
 
  ### Error
Sends message to the console window. The message text is red and prefaced by an error symbol.
Objects that are passed by using the command are converted to a string value.  The stack trace is built in here so that you can easily step through and see where it came from.
 
 `console.error("This is error !");` 
 
  ### Log
Sends message to the console window.
 
 `console.log("Hello World");` 
 
 
## Types of message argument

### Text Message : Multiple aruguments

 Apart from single string message you can also pass in a list of string. The console will treat the arguments as an array and concatenate the output.

 
 `console.log("This", "is", "test", "message");`
 
 ### Object
 
 #### Single Object
 You can not only send string but you can send any object to the console. 
 If you pass an object,  the console window displays it in an object visualizer. You can use the visualizer to inspect properties in the console window.
 
```
var employee = { name: "Dipika", id: 5 };
console.log(employee);
```
 #### Nested Object
 the console window also accepted nested objects and displays it in an object visualizer. You can use the visualizer to inspect properties in the console window.
 
```
var employee = { name: "Dipika", id: 5, address: { line_1: "Mainstreet", City: "Tarrytown", State: "NY"} };
console.log(employee);
```
 #### Multiple Object
 the console window also accepted nested objects and displays it in an object visualizer. You can use the visualizer to inspect properties in the console window.
 
```
var employee = { name: "Dipika", id: 5}
var address  =  { line_1: "Mainstreet", City: "Tarrytown", State: "NY"} };
console.log(employee, address);
```
