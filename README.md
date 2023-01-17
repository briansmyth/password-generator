# Passwordinator
### Generate random passwords of varying complexity

Note : This was a fun project I did when learning. This is not ideal way to generate random passwords and should not be used in any serious applications.
Also, since heroku is down, you might not be able to access the endpoint.

## About

Passwordinator is an API that lets you generate random passwords of varying complexity in your app/website. 
The api is free and can be accessed at any origin.

## How to access

Passwordinator lives at https://passwordinator.onrender.com

End point gives you access to a 14 character long password made of small case alphabets.

### Customization

You can add queries to customize the password

Available queries
- ?num=true ( adds number to the password )
- ?char=true (adds special character to the password )
- ?caps=true ( adds uppercase alphabets to the password )
- ?len=18 ( generates a 18 character password . Must be greater than 7. Default is 12)


## Response format

The API returns a response in json format;

`{ "data" : "sAl7*KladK" }`

## Code example

` fetch('https://passwordinator.herokuapp.com')
.then((res)=> res.json())
.then((data) => console.log(data))
`



`fetch('https://passwordinator.onrender.com?num=true&char=true&caps=true&len=18')`
On resolving generates a 18 digit password with characters, alphabets, uppercase letters and numbers

I will slowly refine the doc. Watchout for new features!


Found this useful? Let's connect on [Twitter](https://www.twitter.com/realfawazsullia)
