# GCPコマンド

1. Storageへのbucketの作成
`<BUCKET_NAME>`はグローバルでユニークであること
    - `gsutil mb gs://<BUCKET_NAME>`

2. ローカルファイルをStorageのbucketにコピー
    - `gsutil cp [MY_FILE] gs://[BUCKET_NAME]`

3. 現在使用可能なリージョンの表示
    - `gcloud compute regions list`

4. 自分のリージョンを環境変数にセット
    - `INFRACLASS_REGION=[YOUR_REGION]`

5. プロジェクトのIDを設定
    - `INFRACLASS_PROJECT_ID=[YOUR_PROJECT_ID]`

6. 環境変数の設定
環境変数用のファイルを作成して追加していく
    - `mkdir infraclass`
    - `touch infraclass/config`
    - `echo INFRACLASS_REGION=$INFRACLASS_REGION >> ~/infraclass/config`
    - `source ~/infraclass/config`
設定を永続的にしたい場合は`~`直下に`.profile`を作成し,最後の行に`source ~\infraclass/config`を追加する
    - `nano .profile`