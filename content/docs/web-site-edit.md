+++
title = 'サイト編集'
date = 2024-04-23T00:31:46+09:00
draft = true
+++

[本サイトについて](./web-site)にあるように以下サイト編集方法を示す。
前提として[環境構築](./web-site-env)が必要となる。
なお、以下コマンドは全てプロジェクトカレントディテクトリ`www %`で行う。


### Fork
元となるリモートリポジトリから自分のリモートリポジトリにコピー

### clone
自分のリモートリポジトリからローカルにブランチごとコピー
git clone git@github.com:あなたのアカウント/www.git

### pull
自分のリモートリポジトリからローカルに同期
```
git pull
```
### リソース新規作成
```
hugo new content docs/web-site-edit.md
```
### [リソース変更](./markup/#markdown)
### 履歴管理状態確認
```
git status
```
### 履歴管理追加
```
git add .
```
### 変更確定
```
git commit -m "#2 add link to fugo."
```
### 変更履歴確認
```
git log
```
### push
ロカールから自分のリモートリポジトリに同期
```
git push
```
### Contribute
pull request