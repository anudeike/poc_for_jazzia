# Sources/Notes

## Creating a Signature using OAuth 1.0
[Twitter Page that explains it](https://developer.twitter.com/en/docs/authentication/oauth-1-0a/creating-a-signature)

**NOTE** It is a little vague on the encoding: it should look like this 
```js
ordered['status'] = encodeURIComponent(ordered['status']).replace(/[!'()*]/g,function(c){
                  return('%'+c.charCodeAt(0).toString(16).toUpperCase());
              });
```

### Check if two strings are the same
[Here](https://text-compare.com/)