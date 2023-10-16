# よくある質問 FAQ

以下は、テストプロジェクトで発生した問題を収集します。それがあなたに役立つことを願っています。

## このシステムでは、ランニングスクリプトが禁止されています

WindowsターミナルツールPowerShellを使用する場合、遭遇する可能性があります。

```bash
ファイルC:\\users\dh\desktop\cs\rename.ps1をロードできません。これは、このシステムでランタイムスクリプトが禁止されているためです。詳細については、https://go.microsoft.com/fwlink/?linkid=135170のabout_execution_policiesを参照してください。

+ CategoryInfo : SecurityError: (:) []，ParentContainsErrorRecordException
+ FullyQualifiedErrorId : UnauthorizedAccess
```

これは、PowerShellの現在の実行戦略が制限されているため（デフォルト設定）、スクリプトファイルを実行することは禁止されています。

**解決：**

管理者を使用してPowerShellを再開し、次のコマンド変更戦略を実行します。

```bash
set-executionpolicy remotesigned
```

## cp 内部または外部コマンドではありません

Windowsに梱包するときは、コマンドラインのエラープロンプトに遭遇する可能性があります。

**解決：**

現在の端子ツールの代わりにGitのインストールで「Git Bash」を使用します。Gitツールをインストールしていない場合は、[ここをクリックしてダウンロード](https://git-scm.com/downloads)インストールしてください。

---

上記は、現在遭遇する可能性のある問題です。他の質問に遭遇した場合は、googleに質問してください。
