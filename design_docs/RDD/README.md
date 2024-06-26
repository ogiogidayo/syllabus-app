## 要件定義
### 機能要件
- ユーザー登録・認証
    - 学生、管理者がアカウントを作成し、ログインできる。
    - メールアドレスとパスワードによる認証が可能。
- シラバス情報の管理
    - ユーザーはシラバスの登録のみができる。
    - 管理者がシラバス情報を登録、編集、削除できる。
- シラバス情報の検索・閲覧
    - 全ユーザーがシラバスを大学名・学部名・授業名で検索できる。
    - シラバスのレビューと評価が見れる。
- レビュー機能
    - ユーザーが授業に対するレビューを投稿できる。
    - レビューにはテキストと評価（１〜５）が含まれる。
    - レビューは他の学生に公開される

### 非機能要件
- lambdaの制約上、ひとつの処理は15分以内に行う
- 処理は同期的に行う

## データベース
### データベース選定
**候補**
- AWS Aurora
- mysql on RDB
- PostgreSQL on RDB
- Dynamo BD