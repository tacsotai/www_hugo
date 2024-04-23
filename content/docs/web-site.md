+++
title = '本サイトについて'
date = 2024-04-20T22:13:19+09:00
draft = false
+++

## 目的
ソフトウェアのエンジニアである私が非エンジニアである協力者に本サイトの内容を編集してもらうことを目的としている。

というのは、急速に発展している領域を仕事にしているものの概念はどんどん変更されていくが、非エンジニアには難しくて通じないことがあるからである。
ある程度歩み寄ってもらうために本サイトを題材にして学んでいただきたい。
|||
|:---|:---|
|初学者へ|[サイト構築基本](../web-basic)|
|編集方法|[サイト編集](../web-site-edit)|  

## サイト構成
本サイトは[Hugo](https://ja.wikipedia.org/wiki/Hugo_(%E3%82%BD%E3%83%95%E3%83%88%E3%82%A6%E3%82%A7%E3%82%A2))という[静的サイト](../web-basic/#静的サイト)ジェネレーター（SSG）を用いて構築している。
それを[Github](https://ja.wikipedia.org/wiki/GitHub)というサイトを通じて[Cloudflare](https://ja.wikipedia.org/wiki/Cloudflare)というサービスの１つであるPagesというWebサーバーにアップロードしている。
![サイト構成](/images/web-site/site-structure.png)

## Hugo
Hugoは[Markdown](../markup/#markdown)を[HTML](../markup/#html)に変換する。内部にWebサーバーを内包しており、作業者が編集状況をHTMLで確認できる。  
![Hugo](/images/web-site/hugo.png)

## Github
Githubは[リソース](../web-basic/#リソース)を共有するための格納庫であるリポジトリをアカウントごとに複数作成することができるクラウドサービスである。
世界中のユーザーが協力して開発することによって大きな成果を生み出している。
![Github](/images/web-site/github.png)

### [git](https://ja.wikipedia.org/wiki/Git)
Githubが使用しているリソースを管理するソフトウェアの１つであり、業界標準（デファクトスタンダード）となっているが、非常に複雑な仕組みとなっている。  
変更を柔軟に戻したり他者とのリソース変更の競合を解決できるようにコピーを量産するためである。  

概念として、１つのリポジトリには複数のbranchがある。 
Github上でリポジトリを作成すると自動的に"master"branchが作成される。
それを元にしてリポジトリごと、またはbranchを（差分）コピーする。
コピーの最小単位はcommitである。 

## Cloudflare Pages
Cloudflare PagesはWebサーバー自体が無料（アクセス数の上限あり）でGithub上のリポジトリ更新で自動的にサイト更新する。  
さらに、Cloudflareは[DNS](../web-basic/#DNS)を提供するのでそのWebサーバーに[サブドメイン](../web-basic/#サブドメイン)を簡単につけることができる。  
また、Hugoだけでなく様々なSSGに対応している。

