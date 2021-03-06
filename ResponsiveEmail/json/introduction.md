# Introduction to the JSON documentation

The ResponsiveEmail API accepts JSON objects as input, and turns these 
objects into responsive emails.

The properties of the email are set in the JSON document. This includes MIME 
headers, alternate versions and optional email attachments. Of course, the most 
important properties are the ones that describe what your email should eventually 
look like: the texts and images that you want to include, and the layout of 
the email.

> **New to JSON?** [Anything you need to know about JSON →](http://www.json.org/)

To give you an idea, the following JSON object contains a simple email with just 
some text:

```javascript
{
    "subject" : "Example document",
    "text" : "This message will show up for clients which are text only.",
    "from" : {
        "address" : "example@responsiveemail.com",
        "name" : "Example"
    },
    "background" : {
        "color" : "white"
    },
    "content" : {
        "blocks" : [{
            "type" : "text",
            "content" : "This is just an example text block."
        }]
    }
}
```

## Top level properties

As you can probably guess from the first example, there are many different 
properties, e.g. `subject`, `text`, `from`, that can be set. These objects can 
even hold arrays and nested data.

[Learn more about top level properties](../json/top-level-properties "Learn more about top level properties")

## The `content` property

The structure and design of emails generated with the API is defined inside the 
property `content`. Here you can add the blocks that will form your responsive 
email, based on a 12 columns grid system.

[Learn more about the content property](../json/property-content "Learn more about the content property")

## The content block types

Emails generated by the ResponsiveEmail.com API are built with blocks. You can 
use text blocks for adding textual content, image blocks for images, columns 
blocks to split your content into multiple responsive columns and many more.

## Example

Add an image

```javascript
{
  "subject" : "Example document",
  "text" : "This message will show up for clients which are text only.",
  "from" : {
    "address" : "example@responsiveemail.com",
    "name" : "Example"
  },
  "content" : {
    "blocks" : [{
      "type" : "image",
      "src"  : "http://placekitten.com/200/140"
      }]
  }
}
```
