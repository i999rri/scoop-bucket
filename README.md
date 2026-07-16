# scoop-bucket (paused)

Scoop bucket for [i999rri/GhosttyWin32](https://github.com/i999rri/GhosttyWin32).

**⚠️ This channel is paused.** The manifest here still points at
`v0.2.2` (the last portable-ZIP release, April 2026). Everything from
`v0.3.0` onward ships as an MSIX + self-signed publisher certificate,
which the current manifest shape can't install, so `scoop install
ghosttywin32` from this bucket will silently give you a stale ZIP build.

Until an established CA / OSS Foundation signature is in place
([GhosttyWin32#46](https://github.com/i999rri/GhosttyWin32/issues/46)),
please install manually from the
[Releases](https://github.com/i999rri/GhosttyWin32/releases) page:

1. Download `Ghostty-<version>-x64.msix` and `Ghostty.cer`
2. Trust the certificate (Local Machine → Trusted People store)
3. Double-click the `.msix` to install

Detailed walkthrough + troubleshooting:
[docs/INSTALL.md](https://github.com/i999rri/GhosttyWin32/blob/main/docs/INSTALL.md).

The bucket will return once signing is available; existing
`scoop bucket add` URLs will keep resolving to this repo, so no
migration will be needed on your end.

<details><summary>日本語</summary>

# scoop-bucket (停止中)

[i999rri/GhosttyWin32](https://github.com/i999rri/GhosttyWin32) の Scoop bucket。

**⚠️ このチャネルは停止中です。** ここの manifest は `v0.2.2` (2026-04 の
portable ZIP 最終リリース) を指したまま。`v0.3.0` 以降は MSIX + 自己署名
証明書配布に切り替わっており、現在の manifest 形状ではインストールできない
ため、このバケットからの `scoop install ghosttywin32` は無音で古い ZIP
ビルドが入るだけになります。

正式な CA / OSS Foundation 署名が入るまで
([GhosttyWin32#46](https://github.com/i999rri/GhosttyWin32/issues/46))、
[Releases](https://github.com/i999rri/GhosttyWin32/releases) ページから
手動でインストールしてください:

1. `Ghostty-<version>-x64.msix` と `Ghostty.cer` をダウンロード
2. 証明書を Local Machine → 信頼されたユーザー ストアに信頼登録
3. `.msix` をダブルクリックしてインストール

詳細手順とトラブルシューティング:
[docs/INSTALL.md](https://github.com/i999rri/GhosttyWin32/blob/main/docs/INSTALL.md)

署名が入り次第 bucket は再開します。既存の `scoop bucket add` URL は
このリポジトリを指し続けるので、ユーザー側でのマイグレーションは不要です。

</details>
