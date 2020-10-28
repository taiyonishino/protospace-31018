# POSTSpaceのER図

## users テーブル

| Column   | Type   | Options     |
| -------- | ------ | ----------- |
| name     | string | null: false |
| email    | string | null: false |
| password | string | null: false |
| profile  | text   | null: false |
|occupation| text   | null: false |
| position | text   | null: false |
 
### Association

## commentsテーブル

| Column  | Type     | Options     |
| ------- | -------- | ----------- |
| text    | text     | null: false |
| users   |references|             |
|prototype|references|             |

### Association

## prototypeテーブル

| Column   | Type     | Options     |
| -------- | -------- | ----------- |
| title    | string   | null: false |
|catch_copy| text     | null: false |
| concept  | text     | null: false |
| image    | ActiveStorageで実践     |
| user     |references|             |

### Association

