# ゼロから始めるJupyter Notebook

![](https://user-images.githubusercontent.com/32427720/65029837-64fbbb00-d979-11e9-8e63-1f28001c4dd4.gif)

## Install

### Windows

Windowsのパッケージマネージャーchocolateyをインストールします．コマンドプロンプトを右クリックから管理者権限で開いて，以下のコマンドを実行してください．

```sh
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```

インストールが終わったら次のコマンドを実行してみてください．このときエラーがでなければインストール成功です．
```sh
choco --version
```

次にanacondaのインストールを行います．次のコマンドを実行してください．(時間がかかる場合があります)

```sh
choco upgrade chocolatey
choco install anaconda3
```

すべてのプログラム(あるいはスタートボタンを右クリック→検索)からanaconda promptを開き，以下を実行してエラーが出ないことを確認してください．

```sh
conda --version
```

### Mac

Mac用のパッケージマネージャーHomebrewをインストールします．command+spaceを押してターミナルと入力して起動してください．次のコマンドをターミナルに張り付けてEnterで実行してください．

```sh
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

途中パスワード聞かれるので，Macのパスワードを入力します．以下のコマンドを実行してバージョンの確認をしてください．

```sh
brew doctor
```

エラーが出なければHomebrewのアップデートを行います．

```sh
brew update --force && brew upgrade
```

次にpythonのインストールを行います．MacはWindowsとは違い，最初からpythonがインストールされているのですが，バージョンが古く(python2系)，また最新のバージョン(python3系)と互換性がないため，新たにインストールする必要があります．

```sh
brew install pyenv
brew reinstall git --with-brewed-curl --with-brewed-openssl
pyenv install anaconda3-5.2.0
```

パスの設定をします．

```sh
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
echo eval "$(pyenv init -)" >> ~/.bash_profile
source ~/.bash_profile
```
anacondaをインストールします．

```sh
pyenv global anaconda3-5.2.0
conda create --name py python=3.6 anaconda
source $PYENV_ROOT/versions/anaconda3-5.2.0/bin/activate py
```

Proceed ([y]/n)?と聞かれたらyを入力してください．

```sh
pyenv versions
```

を実行するとsystemと* anaconda3.5-2.0 (set by /home/usr/.pyenv/version)が出力されると思います．anaconda3.5.2-0のほうに*がついていることを確認してください．最後にanacondaのアップデートをしましょう．

```sh
conda update -y --all
```
