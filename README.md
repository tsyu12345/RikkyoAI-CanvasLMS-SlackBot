# CanvasLMSの課題通知SlackBot

## Poetryのインストール
1. インストール
```bash
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -
```
2. 環境変数の設定
```bash
[System.Environment]::SetEnvironmentVariable('path', $env:USERPROFILE + "\AppData\Roaming\Python\Scripts;" + [System.Environment]::GetEnvironmentVariable('path', "User"),"User")
```


## クローン後開発環境構築手順
1. 仮想環境を作成し、依存関係をインストールする
    ```bash
    $ poetry install
    ```
2. 仮想環境に入る
    ```bash
    $ poetry shell
    ```