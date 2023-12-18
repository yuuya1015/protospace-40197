
## usersテーブル
| Column               | Type   | Options                        |
| ---------------------| -------| -------------------------------|
| email                | string | null: false, unique: true |
| password             | string | null: false                    |
| name                 | string | null: false                    |
| profile              | text   | null: false                    |
| occupation           | text   | null: false                    |
| position             | text   | null: false                    |

##　prototypesテーブル
| Column       | Type       | Options                        |
| -------------| -----------| -------------------------------|
| title        | string     | null: false, foreign_key: true |
| catch_copy   | text       | null: false                    |
| concept      | text       | null: false                    |
| user         | references | null: false                    |

## commentsテーブル
| Column    | Type       | Options                        |
| ----------| -----------| -------------------------------|
| content   | text       | null: false                    |
| prototype | references | null: false, foreign_key: true |
| user      | references | null: false, foreign_key: true |


### Association
- belongs_to : #仮置き
- belongs_to :user #仮置き