# What's this?

CLIからwindowsの音声出力デバイスを変更できるツール

ショートカットなどを作成すれば、ボタン1つで出力デバイスを変更できます。

# 動作環境

以下のバージョンでの動作を確認
- powershell 7.4.0

# 使い方

- `deviceList.ps1`を実行し、デバイスのリストを取得

  ```powershell
  PS C:\audioDeviceSet> .\deviceList.ps1
    Active Sound devices:
    ヘッドセット イヤフォン
        \{13be39b7-cadc-454d-84f7-a36f44e12e8f}
    ヘッドホン
        \{4d69322b-fbf6-4b94-af6e-f56ab9fa9067}
  ```

- `deviceSet.ps1`を実行し、出力デバイスを変更

  ```powershell
  PS C:\audioDeviceSet> .\deviceSet.ps1 "{4d69322b-fbf6-4b94-af6e-f56ab9fa9067}"
  SUCCESS: The default audio device has been set.
  ```

# 備考

中身はすべて[参考リンクの1つ目](#参考)となっています。

なお、このリポジトリの作成者と参考ページを書いた方は別人です。

# 参考

https://itib.hatenablog.com/entry/2021121001

https://litera.app/blog/windows-setting-shortcut/
