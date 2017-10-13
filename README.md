# dotenv-kv

This would have the ability to load an .env file or just a file with key value pairs, exclude new lines and comments by default! No need to remove all the equal signs in the file!

### Expected Behavior

##### Input:: Given a file `.env` file

```json
// Just a comment
FILE=2303
NEW=2019

//
SAMPLE=4015
```

`run load .env` should write all key value  with the format “chamber load someservice key value |-> ”

##### Expected output:
```json
chamber load someservice FILE 2303 |->
chamber load someservice NEW 2019 |->
chamber load someservice SAMPLE 4015 |->
```
