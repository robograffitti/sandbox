#超簡略チートシート

##コマンドライン

> $ ls -a

lsでカレントディレクトリのファイル一覧が見られる。-aオプションで隠しファイルも見える。

> $ cd (dir name)

移動したいディレクトリを指定するとchange directoryできます。めっちゃ使う。  
../で一つ上に移動できます。

> $ touch (file name)

適当なファイルを作れます

> $ mkdir (dir name)

適当なディレクトリを作れます


##GitHub 初期設定

###Config

アカウントの設定です。ターミナルからコマンドを打ちます。

> $ git config --global user.name "hogehoge"

> $ git config --global user.email "hogehoge@exapmle.com"

###SSHの設定

鍵を作成します。以下コマンド。

> $ ssh-keygen

これで id_rsa, id_rsa.pubみたいなのができます。それぞれ秘密鍵と公開鍵です。公開鍵をGitHubに登録してください。

##GitHub使い方

###clone

リモート（GitHub）にあるリポジトリをローカル（手元のPC）にクローンします。  
このリポジトリをクローンする場合はローカルの適当なディレクトリ（どこでもいい）で以下のコマンドを実行

> $ git clone https://github.com/ut-marukyu/sandbox.git

続けて

> $ git cd RepositoryTest

でディレクトリ移動します。

> $ ls -a

をすると.gitという隠しフォルダがあると思います。この.gitがあるディレクトリがリポジトリとなります。

###pull

他の人が書き換えたりなどして、リモートに変更があった場合はpullするとローカルを更新できます。

> $ git pull

###add, commit, push

ローカルのファイルを変更後

> $ git add .

> $ git commit -m 'hogehoge'

> $ git push

のコマンドを打つとリモートに反映されます。

###others

mergeとかbranchとか新しいリポジトリ作成とかは適宜更新





