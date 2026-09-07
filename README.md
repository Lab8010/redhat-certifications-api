# Red Hat Certification List

This repository provides a machine-readable list of Red Hat certification information, published in multiple formats (JSON, YAML, CSV).  
Ideal for developers, instructors, and anyone who wants to programmatically access Red Hat's certification catalog.

---

このリポジトリは、Red Hat認定資格の一覧を機械可読な形式（JSON、YAML、CSV）で提供するものです。  
開発者、講師、認定制度に関心のある方が、資格情報をプログラム的に活用できるように設計されています。

---

## 🔍 Available Formats | 利用可能なフォーマット

| Format | File Path |
|--------|-----------|
| JSON   | `data/certifications.json` |
| YAML   | `data/certifications.yaml` |
| CSV    | `data/certifications.csv` |
| Tracks | `data/tracks.json` |

You can access these directly via GitHub Raw or use them in your own apps.  
これらのファイルはGitHubのRawリンクを使って直接アクセスすることも、自作アプリケーションに組み込むことも可能です。

`tracks.json` には、Red Hat公式の製品トラック（OpenShift、Enterprise Linux、Ansible、Cloud-native applications、AI）と、TechnologistからArchitectまでの取得対象試験を収録しています。資格一覧はRed Hat公式ページを基準に更新しています。

---

## 🌐 GitHub Pages (UI View)

A simple browser interface is available at:

https://lab8010.github.io/redhat-certifications-list/


ブラウザで閲覧できる簡易インターフェースも上記URLで提供されています（GitHub Pagesを有効化してください）。

### 🖥️ Local Development | ローカル開発

To run the HTML interface locally, start a local HTTP server:

ローカルでHTMLインターフェースを実行するには、ローカルHTTPサーバーを起動してください：

```bash
# Python 3の場合
cd docs
python3 -m http.server 8000

# Node.jsの場合（http-serverが必要）
cd docs
npx http-server -p 8000
```

Then open `http://localhost:8000/index.html` in your browser.

その後、ブラウザで `http://localhost:8000/index.html` を開いてください。

**Note:** The HTML file uses `fetch()` to load JSON data, which requires an HTTP server. Opening the file directly (`file://`) will result in CORS errors.

**注意:** HTMLファイルは`fetch()`を使用してJSONデータを読み込むため、HTTPサーバーが必要です。ファイルを直接開く（`file://`）とCORSエラーが発生します。

---

## 📦 Use Cases | 活用例

- Build your own dashboard of certifications
- Create Slack bots or chat integrations
- Enable auto-fetch in training systems
- GitHub Actionsで定期的に更新して、常に最新の資格一覧を共有
- 資格カタログのデータソースとして他のツールと連携

---

## 🤝 Contributing | コントリビュート歓迎

If you'd like to add more certifications, fix data, or improve formatting, feel free to open a pull request.  
資格情報の追加や修正、フォーマットの改善など、どなたでもPull Requestで貢献いただけます。

---

## 📜 License

This repository is provided under the [MIT License](LICENSE).  
（※必要に応じて適切なライセンスを明記してください）

---

Maintained by [@Lab8010](https://github.com/Lab8010)
