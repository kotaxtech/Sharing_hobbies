# Sharing_hobbies

### 概要
- 趣味を共有・発信できるWEBアプリケーション。
### 目的
- プログラミングコミュニティ内の学生同士を仲良くさせること。
### 開発期間
- 1日間
### 人数
- 3人
### 苦労した点
- 初ハッカソンであったため、適切な時間配分や実装箇所の選別が苦労した。
### 学んだこと
- 短期間のハッカソンであれば、アイデアベースで開発することも重要であること。
- アプリを使うことでユーザーにとって、どんなメリットがあるのかが重要であること。


# デモ

発表スライド上にあります。

https://docs.google.com/presentation/d/1wKyySZ5vkTtHVxvYOetI5jQwDg533bjwxP6qcDDvd4c/edit?usp=sharing


# 使い方
### Githubからclone
Github上からソースコードをローカルPC上にcloneします。
```
$ git clone git@github.com:K-out-A/Sharing_hobbies.git
```
cloneしたディレクトリ上に移動します。
```
$ cd Sharing_hobbies
```

### 動作環境の構築
仮想環境を作成します。（そのまま実行すると既存のパッケージに干渉してエラーが起きる可能性があるためです。）
```
$ python3 -m venv myvenv
```
仮想環境を実行します。
```
$ source myvenv/bin/activate
```
必要なライブラリを仮想環境上にinstallします。（requirements.txtの中に必要なライブラリのリストが入っています。）
```
$ pip3 install -r requirements.txt
```

### ソースコードの実行
以下のコードを順に実行します。
```
$ python3 manage.py makemigrations

$ python3 manage.py migrate

$ python3 manage.py runserver
```

http://127.0.0.1:8000/ にアクセスして、デモ動画の冒頭ページが表示されたら成功です。

### WEBアプリで発信
WEBアプリにログインします。

チャネルをクリックし、『新規』から趣味を発信します。

※「マンガ」「アニメ」「恋愛」「スポーツ」の4チャネルから投稿できます。


# 動作環境の詳細
- Python 3.7.3
- Django 3.1.2
