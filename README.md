#ProtoSpaceのER図

## usersテーブル
| Column     | Type     | Option      |
| ---------- | -------- | ----------- |
| email      | string   | null: false |
| password   | string   | null: false |
| user_name  | string   | null: false |
| profile    | text     | null: false |
| occupation | text     | null: false |
| position   | text     | null: false |

## prototypesテーブル
| Column     | Type      | Option            |
| ---------- | --------- | ----------------  |
| title      | string    | null: false       |
| catch_copy | text      | null: false       | 
| concept    | text      | null: false       |
| ※image     |           | Active_Storageで実装 |
| user       | reference |                   |

## commentsテーブル
| Column    | Type       | Option           |
| --------- | ---------- | ---------------- |
| text      | text       | null: false      |
| user      | reference  | null: false      |
| prototype | reference  | null: false      |
