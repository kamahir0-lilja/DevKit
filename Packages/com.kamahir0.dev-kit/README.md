# Lilja DevKit

[![license](https://img.shields.io/badge/LICENSE-MIT-green.svg)](LICENSE)
![unity-version](https://img.shields.io/badge/unity-6000.0+-blue.svg)

Development toolkit, package creator, and templates for Lilja Unity packages.

---

## 📦 インストール方法

### Package Manager (Git URL)

Unity Editorの **Package Manager > [+] > Add package from git URL...** に以下を入力します：

```text
https://github.com/kamahir0-lilja/DevKit.git?path=/Packages/com.kamahir0.dev-kit
```

特定のバージョンを指定する場合は、末尾にタグを付加してください（例: `#vcom.kamahir0.dev-kit`）。

### manifest.json による導入

プロジェクトの `Packages/manifest.json` の `dependencies` に直接追加することも可能です：

```json
{
  "dependencies": {
    "com.kamahir0.dev-kit": "https://github.com/kamahir0-lilja/DevKit.git?path=/Packages/com.kamahir0.dev-kit"
  }
}
```

---



## 📖 基本的な使い方

```csharp
using Lilja.DevKit;
```

---

## 🛠️ 開発・検証方法

本リポジトリ自体が独立したUnityプロジェクトになっています。Unity Hubから本リポジトリのルートフォルダを開くことで、開発および動作確認が可能です。

- 配布対象パッケージ本体: `Packages/com.kamahir0.dev-kit/` (Embedded Package)
- 開発・動作検証用コード: `Assets/Development/`

---

## 📄 ライセンス

[MIT License](LICENSE)
