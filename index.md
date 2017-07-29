# SyncSpot API documentation version 1.0
https://app.thesyncspot.com/api/v1

---

## /login
login with password

### /login

* **post**: 

## /logout

### /logout

* **get**: 

## /setpassword
Temp method to set password

### /setpassword

* **post**: 

## /signin/facebook
Sign in using Facebook account

### /signin/facebook

* **get**: 

## /sign/gplus
Sign in using Google account

### /sign/gplus

* **get**: 

## /resetemail
Send email with password reset link

### /resetemail

* **get**: 

## /resetpassword
Generate password and send to email

### /resetpassword

* **get**: 

## /confirm
Confirm email

### /confirm

* **get**: 

## /login/authorizeClient
System/embeded browser should be started client auth with following URL

### /login/authorizeClient

* **get**: 

## /login/setClientId
Set clientId authorization, sends frontend after sign in. Parameters fetch from cookies.

### /login/setClientId

* **get**: 

## /login/exchangeId
Exchange initial clientId on auth token

### /login/exchangeId

* **get**: 

## /register

### /register

* **post**: 

## /register/confirm
Confirm profile's email

### /register/confirm

* **get**: 

## /sync/contacts
Get current sync process state

### /sync/contacts

* **get**: 

## /sync/contacts/all
Sync all active

### /sync/contacts/all

* **get**: 

## /sync/contacts/google
Import contacts (deprecated)

### /sync/contacts/google

* **get**: 

## /sync/contacts/ios

### /sync/contacts/ios

* **post**: Send contacts
* **get**: Get contact changes

## /sync/contacts/ios/open
Get contact changes, set opened transaction

### /sync/contacts/ios/open

* **get**: 

## /sync/contacts/ios/close
Close transaction. If transaction is opened, PUT [Contacts] is not acceptable and get contacts always return the same (the last transaction message).

### /sync/contacts/ios/close

* **post**: 
* **put**: 

