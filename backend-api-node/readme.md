## Introduction

run mongodb locally mac
------------------------
- brew services start mongodb
Then access the shell by
- mongo
You can shut down your db by
- brew services stop mongodb
You can restart your db by
- brew services restart mongodb
For more options
- brew info mongodb

### Install the Dependencies

    npm i

### Populate the Database

    node seed.js

### Run the Tests

You're almost done! Run the tests to make sure everything is working:

    npm test

### Start the Server

    node index.js

http://localhost:3900/api/genres


### (Optional) Environment Variables

If you look at config/default.json, you'll see a property called jwtPrivateKey. This key is used to encrypt JSON web tokens. So, for security reasons, it should not be checked into the source control. Someone has set a default value here to make it easier for you to get up and running with this project. For a production scenario, you should store this key as an environment variable.

On Mac:

    export vidly_jwtPrivateKey=yourSecureKey

On Windows:

    set vidly_jwtPrivateKey=yourSecureKey
