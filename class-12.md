# This is my journal 5/24/2022

## What I have learned today

- Today I learned about JSON and local storage.

> JavaScript Object Notation is a schema-less, text-based representation of structured data that is based on key-value pairs and ordered lists. Although JSON is derived from JavaScript, it is supported either natively or through libraries in most major programming languages. JSON is commonly, but not exclusively, used to exchange information between web clients and web servers. (https://www.infoworld.com/article/3222851/what-is-json-a-better-format-for-data-exchange.html)

- JSon has become integral to web development. It is the format of choice for most private web services.

- The popularity of JSon has made it so many data bases natively support JSON. NoSQL and MONGODB and Neo4j also support JSON.

> This is an example of data recorded in JSON: 
{
  “firstName”: “Jonathan”,
  “lastName”: “Freeman”,
  “loginCount”: 4,
  “isWriter”: true,
  “worksWith”: [“Spantree Technology Group”, “InfoWorld”],
  “pets”: [
    {
      “name”: “Lilly”,
      “type”: “Raccoon”
    }
  ]
}
<!-- (https://www.infoworld.com/article/3222851/what-is-json-a-better-format-for-data-exchange.html) -->

- Json data is stored in files that end with the json extension.

- XML is an alternative to JSON, but it is becoming less and less popular. In addition to being less dry, XML also makes it more difficult to parse Javascript.

> JSON is a fairly concise language that works with many languages however there are some drawbacks: no schema, only one number type,no date type, no comments, verbosity.

- If you are writing software that communicates with browsers or mobile applications you should use the JSon data format. XML is out of date won't work well these days.

- Javascript has a native JSON parser JSON.parse(). Strong typed languages need a little more work to be done to be compatible with JSON.

- JSONlint will format and validate arbitrary JSONcode, JSON viewer creates an interactive tree to help you understand code. JSON beautifier will help you pretty print your code.   JSON converter helps you quickly move data from JSON to something else.

>This is where local storage comes in. You would keep a key on the user’s computer and read it out when the user returns. The classic way to do this is by using a cookie. A cookie is a text file hosted on the user’s computer and connected to the domain that your website runs on. You can store information in them, read them out and delete them. Cookies have a few limitations though: 
<!-- https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/ -->

- Using local storage in modern browsers is simple, you just need to modify local storage in Javascript. You can do that with the setItem() and getItem()

Example: localStorage.setItem('favoriteflavor','vanilla');
Example2: localStorage.removeItem('favoriteflavor');

You can work around this by using the native JSON.stringify() and JSON.parse()
