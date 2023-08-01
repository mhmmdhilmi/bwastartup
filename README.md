## Entity analysis

- Users
- Campaigns
- Campaign Images
- Transactions 

## Field analysis

#### - Users
* id : int
* name :  varchar
* occupation : varchar
* email : varchar
* password_hash : varchar
* avatar_file_name : varchar
* role : varchar
* token : varchar
* created_at : datetime
* updated_at : datetime

#### - Campaigns
* id : int
* user_id : int
* name : varchar
* short_description : varchar
* description : text
* goal_amount : int
* current_amount : int
* perks : text
* backer_count : int
* slug : varchar
* created_at : datetime
* updated_at : datetime

#### - Campaign Images
* id : int
* campaign_id : int
* file_name : varchar
* is_primary : boolean (tinyint)
* created_at : datetime
* updated_at : datetime

#### - Transactions
* id : int
* campaign_id : int
* user_id : int
* amount : int
* status : varchar
* code : varchar
* created_at : datetime
* updated_at : datetime

## library
gin (http framework)
```go get -u github.com/gin-gonic/gin```

gorm (database access)
```go get -u gorm.io/gorm```
```go get -u gorm.io/driver/sqlite```


