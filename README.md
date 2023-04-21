# Haikus for Codespaces

[GitHub Codespaces のクイックスタート - GitHub Docs](https://docs.github.com/ja/codespaces/getting-started/quickstart)
を見ながら試した GitHub Codespaces の練習。

中身は [express](https://www.npmjs.com/package/express)
を使ったちょっとしたサーバで、
ポートが転送されてローカルで見れるのがすごい。

あと

* 個人的な好みで pnpm に 変えた。
* secret置いてみた。codespacesのディスク上に.envに書かれた秘密が残る(消さない限り)。

```
$ pwd
/workspaces/haikus-for-codespaces

$ uname -a
Linux codespaces-bb4403 5.4.0-1105-azure #111~18.04.1-Ubuntu SMP Fri Mar 3 22:47:43 UTC 2023 x86_64 x86_64 x86_64 GNU/Linux

$ ls -la ~
total 120
drwxrwsr-x 1 codespace codespace 4096 Apr 21 01:27 .
drwxr-xr-x 1 root      root      4096 Apr 21 01:13 ..
-rw-rw-r-- 1 codespace codespace  220 Feb 25  2020 .bash_logout
-rw-rw-r-- 1 codespace codespace 5226 Apr  3 22:31 .bashrc
drwxrwsr-x 1 codespace codespace 4096 Apr 21 01:24 .cache
drwxr-sr-x 4 codespace codespace 4096 Apr 21 01:14 .config
lrwxrwxrwx 1 root      codespace   47 Apr 21 01:15 .docker -> /workspaces/.codespaces/.persistedshare/.docker
lrwxrwxrwx 1 codespace codespace   25 Apr  3 22:50 .dotnet -> /usr/local/dotnet/current
drwxrwsr-x 2 codespace codespace 4096 Apr  3 22:50 .hugo
drwxrwsr-x 1 codespace codespace 4096 Apr  3 22:38 .jupyter
drwxrwsr-x 1 codespace codespace 4096 Apr  3 22:38 .local
drwxrwsr-x 2 codespace codespace 4096 Apr  3 22:50 .maven
drwxrwsr-x 1 codespace codespace 4096 Apr  3 22:47 .minikube
drwxrwsr-x 1 codespace codespace 4096 Apr 21 01:14 .npm
drwxrwsr-x 1 codespace codespace 4096 Apr  3 22:34 .nvs
drwxrwsr-x 1 codespace codespace 4096 Apr  3 22:31 .oh-my-zsh
drwxrwsr-x 2 codespace codespace 4096 Apr  3 22:50 .php
-rw-rw-r-- 1 codespace codespace  807 Apr  3 22:31 .profile
drwxrwsr-x 2 codespace codespace 4096 Apr  3 22:50 .python
drwxrwsr-x 1 codespace codespace 4096 Apr  3 22:46 .rbenv
drwxr-sr-x 2 codespace codespace 4096 Apr 21 01:27 .redhat
drwxrwsr-x 2 codespace codespace 4096 Apr  3 22:50 .ruby
-rw-r--r-- 1 codespace codespace   39 Apr 21 01:13 .rvmrc
drwxr-sr-x 5 codespace codespace 4096 Apr 21 01:14 .vscode-remote
-rw-rw-r-- 1 codespace codespace 3903 Apr  3 22:31 .zshrc
lrwxrwxrwx 1 codespace codespace   33 Apr  3 22:50 java -> /usr/local/sdkman/candidates/java
lrwxrwxrwx 1 codespace codespace   20 Apr  3 22:50 nvm -> /usr/local/share/nvm

$ node -v
v19.8.1

$ go version
go version go1.20.2 linux/amd64

$ python --version
Python 3.10.4

$ java -version
openjdk version "17.0.6" 2023-01-17 LTS
OpenJDK Runtime Environment Microsoft-7209853 (build 17.0.6+10-LTS)
OpenJDK 64-Bit Server VM Microsoft-7209853 (build 17.0.6+10-LTS, mixed mode, sharing)

$ cargo -v
bash: cargo: command not found
```

rustは入ってないのね...

ちょっとプロンプトが長いので、何か考える。
