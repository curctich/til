# git cloneしたリポジトリを別リポジトリにPUSHする

1. `git clone`を実行

```
$ git clone git@github.com:ユーザー/リポジトリ名.git リポジトリの別名
```

---

2. GitHubで新リポジトリ作成しURLを取得

---

3. gitのremote url変更

```
$ cd リポジトリ
```

- **remote urlの確認**
```
$ git config remote.origin.url
```
=> 「git@github.com:ユーザー/リポジトリ名.git」が表示される

<br>

- **remote urlの変更**
```
$ git remote set-url origin git@github.com:ユーザー/リポジトリ名.git
```

<br>

- **remote urlの確認**
```
$ git config remote.origin.url
```
=> 「git@github.com:ユーザー/リポジトリ名.git」が表示される

---

4. 新リポジトリにpush
```
git push
```