# 課題② - 実施すること
## 1. GitHubアカウントを作成する
## 2. Gitに下記を設定する
    * git config --global init.defaultBranch main
    * git config --global user.name "ユーザー名"
    * git config --global user.email "メールアドレス"
## 3. コースの課題を格納する為のリポジトリを作成する(Public)
## 4. 「ブランチ:lecture02」を作成して、今回の講座で学んだことを「 lecture02.md 」に Markdownで記載
## 5. プルリクエストを発行する
<br>

# 課題② - 学んだこと
## 1. Gitについて  
ファイルのバージョン管理に使用される仕組みのこと。  
リポジトリと呼ばれるファイルの保管場所にファイルとその変更履歴を保存しておき、変更履歴を活用することでファイルをいつでも好きな状態に変更することが可能となっている。
分散型バージョン管理システムというものを採用しており、オンライン上とローカルの2つの環境にリポジトリを用意することで耐障害性の高いファイル管理の仕組みを実現している。  
リポジトリはオンライン上⇔ローカルとで好きなタイミングで同期させることができる。  
<br>
<br>

## 2. GitHubについて  
Gitで使用するリポジトリをオンライン上に配置し、そのリポジトリをコピーすることで複数人でのファイルの編集を可能とする仕組みのこと。  
Gitはファイルのバージョン管理システムそのものを指し、GitHubはGitを複数人で共有するWebサービスのこと。
<br>
<br>

# 課題② - プルリクエストまで
1. GitHub上に「lecture02」リポジトリを作成
2. ローカルとリモートリポジトリ間でssh認証を設定
3. 「git clone git@github.com:ユーザ名/リポジトリ名.git」にて、リモートリポジトリをローカル環境に複製
4. ローカル環境に配備したリポジトリ配下に「lecture02.md」を作成  
5. 「lecture02.md」をステージ⇒コミット
   * git add lecture02
   * git commit -m 'メッセージ' lecture02.md
6. 「lecture02」ブランチを作成し、カレントブランチを変更
   * git branch lecture02
   * git checkout lecture02
7. 「main」ブランチをGitHub上にpush
   * git push origin main
8. 「lecture02.md」を修正
9. 「lecture02」ブランチをGitHub上にpush
10. プルリクエストを送信
