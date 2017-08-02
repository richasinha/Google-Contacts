Node.js wrapper for the Google Contacts API.

# This is not the actual google-contacts node-js support library
I had to create an app as a part of my project and I came across this. It supports retrieving contact but not create, delete and update so as per my requiremnt I made the changes. 

You can use this as per your requirement and let me know if my there are any issues. 

# Install

```
npm install google-contacts
```

# Usage

```javascript
var GoogleContacts = require('google-contacts').GoogleContacts;
var c = new GoogleContacts({
  token: 'oauth2 token...'
});

c.getContacts(cb, params);

```

Params:

**type** (default: 'contacts')
**alt** (default: json)
**projection**
**email** (default: 'default')
**max-results** (default: 2000)

See [https://developers.google.com/google-apps/contacts/v3/](https://developers.google.com/google-apps/contacts/v3/).

# Test

```
 GOOGLE_TOKEN=sometoken npm run test
 # verbose test
 DEBUG=google-contacts GOOGLE_TOKEN=sometoken npm run test
```

You can get a test token at [https://developers.google.com/oauthplayground/](https://developers.google.com/oauthplayground/).
