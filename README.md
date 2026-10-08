# LonStudio Downloads

LonStudio（Windows版）の公式配布ファイルを置いているリポジトリです。
ソースコードは含まれていません。配布ファイルは [Releases](../../releases) にあります。

- 公式サイト: https://www.lonstudio.workers.dev
- ダウンロード: https://www.lonstudio.workers.dev/download
- お問い合わせ: https://www.lonstudio.workers.dev/support

## ダウンロード方法

**公式サイトの [Download](https://www.lonstudio.workers.dev/download) から `LonStudio_Downloader.exe` を取得して起動してください。**

インストーラーは 2GB 未満の複数のファイル（`.exe` 1 個と `.bin` 9 個、合計 約17.3GB）に分かれています。
LonStudio Downloader が、すべてのファイルをこのリポジトリの Release から取得し、
署名されたダウンロード情報と全ファイルの SHA-256 を確認してから、インストーラーを起動します。
途中で止めても、次回は続きから再開します。

手動でダウンロードする場合は、Release の `LonStudio_Setup_1.0.0.exe` と
`LonStudio_Setup_1.0.0-1.bin` ～ `-9.bin` を**すべて同じフォルダー**に保存し、
`SHA256SUMS.txt` と一致することを確認してから `LonStudio_Setup_1.0.0.exe` を実行してください。

## 動作環境

- Windows 11（64bit）
- NVIDIA製GPU（VRAM 8GB以上を推奨）と対応するドライバー
- 空き容量：インストール先のCドライブに約45GB（インストーラーの保存先を含めて70GB以上を推奨）
- インターネット接続

## 無料体験とライセンス

ダウンロードとインストールに購入は必要ありません。インストール後は無料体験として利用できます。
製品版（買い切り）のライセンスキーは、公式サイトの案内に沿って購入後にお渡しします。
LonStudio の「ライセンスキーを認証」に入力すると製品版になります。

## 「Windows によって PC が保護されました」と表示された場合

`LonStudio_Downloader.exe` と `LonStudio_Setup_1.0.0.exe` にはコード署名がありません。
初回の起動時に Microsoft Defender SmartScreen の確認画面が表示されることがあります。
「詳細情報」→「実行」を選ぶと続行できます。
心配な場合は、ファイルの SHA-256 が Release に記載の値と一致することを確認してください。

```powershell
Get-FileHash .\LonStudio_Setup_1.0.0.exe -Algorithm SHA256
```

## ライセンス

LonStudio は有償のソフトウェアです。利用条件は [利用規約](https://www.lonstudio.workers.dev/terms) をご覧ください。
同梱している第三者ソフトウェアのライセンスは、インストール後のフォルダーにある `THIRD_PARTY_NOTICES.txt` に記載しています。
