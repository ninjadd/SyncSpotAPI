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

## /sync/contacts/outlookagent

### /sync/contacts/outlookagent

* **post**: Send contacts
* **get**: Get contact changes

## /sync/state

### /sync/state

* **get**: Get datasources sync state

### /sync/state/{datasource}

* **get**: Wait 1 minute for a successful plugin authorization

### /sync/state/{datasource}/{state}

* **post**: If state=3 then wait for sync not more than 1 minute then return

## /signin/getgooglephoto
get google avatar photo

### /signin/getgooglephoto

* **get**: 

## /contact
Create new user's contact

### /contact

* **post**: 

### /contact/list
Get user's contacts

* **post**: 

### /contact/filters
Get all possible filter's values

* **post**: 

### /contact/inviteList

* **get**: Get contacts for invitation list
* **post**: Send invitations

### /contact/{contactId}

* **get**: 
* **put**: Update conact
* **delete**: Delete contact

### /contact/{contactId}/phone

* **get**: 
* **post**: 

### /contact/{contactId}/phone/{phoneId}

* **put**: 
* **delete**: 

### /contact/{contactId}/email

* **get**: 
* **post**: 

### /contact/{contactId}/email/{emailId}

* **put**: 
* **delete**: 

### /contact/{contactId}/addresses

* **get**: 
* **post**: 

### /contact/{contactId}/addresses/{addressId}

* **put**: 
* **delete**: 

### /contact/{contactId}/photoLinks

* **get**: 
* **post**: 

### /contact/{contactId}/photoLinks/{photoLinkId}

* **put**: 
* **delete**: 

### /contact/{contactId}/webSites

* **get**: 
* **post**: 

### /contact/{contactId}/webSites/{webSiteId}

* **put**: 
* **delete**: 

## /activity

### /activity

* **post**: Get activity using filters from SearchParam

### /activity/{contactId}

* **post**: Get activity for contactId

## /profile

### /profile

* **get**: Get profile details
* **put**: Update profile details (also after a first sign-in)
* **delete**: Delete profile and it's contacts

### /profile/statistics
Get profile statistics

* **get**: 

### /profile/types/addresses

* **get**: Get address types
* **post**: Create new address type

### /profile/types/addresses/{addressTypeId}

* **delete**: Delete custom address type

### /profile/types/emails

* **get**: Get email types
* **post**: Create new email type

### /profile/types/emails/{emailsTypeId}

* **delete**: Delete custom email type

### /profile/types/phones

* **get**: Get phone types
* **post**: Create new phone type

### /profile/types/phones/{phonesTypeId}

* **delete**: Delete custom phone type

## /dupes

### /dupes

* **get**: Collect duplicates

### /dupes/{filter}/shift

* **get**: Get suspected duplicates

### /dupes/{filter}/shift/select/{contactIndexAmongDupes}

* **post**: Select contact

### /dupes/{filter}/shift/delete/{contactIndexAmongDupes}

* **post**: Not a duplicate

### /dupes/{filter}/shift/merge

* **post**: Merge contacts

## /photo?href={imageId}
Get photo

### /photo?href={imageId}

* **get**: Get photo

## /search
Search contacts by name

### /search

* **post**: Search contacts by name

## /feedback/learnmore
Send "Learn more" frorm a landing page

### /feedback/learnmore

* **post**: Send "Learn more" frorm a landing page

