# 環境設定
## 1.Gitに登録する
### 1-1.gitに登録されているか確認する
以下のコマンドをターミナルに入力してください。
`git config --global --list`

```commandLine
super@supakonpyuta NWS % git config --global --list
user.name=example
user.email=example@example.com
```
`user.name`と`user.email`の欄にユーザー名とアドレスが入っていたら、1.Gitに登録するはクリア。
設定されていなかったら、`1-2.Gitにユーザー名を登録する`にしてください。

### 1-2.Gitにユーザー名を登録する
以下のコマンドをターミナルに入力してください。
`git config --global user.name <username>`

### 1-3.Gitにメールアドレスを登録する
以下のコマンドをターミナルに入力してください。
`git config --global user.email <emailaddress>`

## 2.リポジトリをローカルにクローンする
### 2-1.クローンする
以下のコマンドをターミナルに入力してください。
`git clone https://github.com/sp-DEGU/NWS.git`

## 3.rubyのインストール
### 3-1.rubyのバージョンを確認する
ターミナルで以下のコマンドを入力するとrubyのバージョンを確認できます。
このプロジェクトでは、rubyのバージョンは`2.6.6`です。
`rbenv versions`

#### ・rubyのバージョンは2.6.6の時
```commandLine
super@supakonpyuta NWS % rbenv versions
  system
  2.6.5
* 2.6.6
```
`2.6.6`のところに`※`があったら、1.rubyのインストールは、終了です！

#### ・2.6.6はインストールされているが、設定されていない場合
```commandLine
super@supakonpyuta NWS % rbenv versions
  system
* 2.6.5
  2.6.6
```
`2.6.6`は表示されているが、`*`が違うバージョンにあったら以下のコマンドを入力してください
`rbenv local 2.6.6`
このコマンドでrubyのバージョンが`2.6.6`になり、1.rubyのインストールは、終了です！

### 3-2.rubyをインストールする
#### 2.6.6をインストールする
ターミナルで以下のコマンドを入力するとインストールできます。
`rbenv install 2.6.6`

#### 環境で2.6.6を使えるようにする
環境全体で`2.6.6`を指定したい場合
`rbenv global 2.6.3`
or
特定のプロジェクトだけで`2.6.6`を指定したい場合
`rbenv local 2.6.3`

#### 使えるようになっているか確認する
ターミナルで以下のコマンドを入力して、`* 2.6.6`になっていたらOKです。
`rbenv versions`

### 3-3.gemのインストールする
#### gemをインストールする
ターミナルで以下のコマンドを入力するとインストールを開始します！
`gem install bundler`

#### bundleをインストール
ターミナルで以下のコマンドを入力するとインストールを開始します！
`bundle install`

## 4.railsをインストールする
#### 6.0.3.2をインストールする
ターミナルで以下のコマンドを入力してください。
`gem install rails -v "6.0.3.2"`

#### インストールされているか確認する
ターミナルで以下のコマンドを入力してください。
`rails -v`

## 5.SCSSをインストール
#### SCSSをインストールする
`sudo gem install sass`

#### インストールされているか確認する
ターミナルで以下のコマンドを入力してください。
`sass -v`


