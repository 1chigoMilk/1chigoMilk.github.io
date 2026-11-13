ちるたいむBot公式サイト — 作業引継ぎ README
資料版: V26.11.13.1728
対象リポジトリ: 1chigoMilk/1chigoMilk.github.io
対象サイト: Ch1llTimeBotOfficialSite/
メインページ: Ch1llTimeBotOfficialSite/index.html
正規ブランチ: main
全面改修コミット: d54d0ed0c9afc4f13e0877ff3c66609cb247031b
改修後 index.html blob SHA: 2b4db11a0e71bc744d69675de274efe075a41029

【このREADMEの目的】
次のChatGPTセッション・別の開発環境で、既存サイトのデザイン・説明・規約・リンク・画像を欠落させることなく、開発を続けるための引継ぎです。

【正本とファイル構成】
・正本はGitHub 1chigoMilk/1chigoMilk.github.io の main ブランチ。
・サイトの本体は Ch1llTimeBotOfficialSite/index.html。
・既存のメインビジュアルはindex.htmlにWebP data URIとして内包されている。見た目だけでなく画像データの完全性を維持する。
・仕様書_V26.11.13.1728.txt：ページ構成・利用者向け文面・設計思想。
・作業報告書_V26.11.13.1728.txt：原文依頼・変更内容・検証・未完了。
・リポジトリ全体を引き継ぐ場合、GitHubの「Code」→「Download ZIP」から取得し、元の階層を保存する。サイトのHTMLだけに限定したアーカイブを完全なリポジトリと誤認しない。

【変更履歴／設計意図】
1. 旧サイトの簡素な機能紹介・3段階導入・FAQ4件を、11セクションの包括的なサイトへ再設計。
2. 機能紹介6種、通常・β・Xの3ルート、メッセージ例4種、導入4ステップ、技術の説明、安全性の説明、FAQ13件へ整理。
3. 法的説明の全文を残しつつ、長大な一括表示をdetails/summaryの折りたたみUIへ構造変換。
4. プライバシーポリシーの外部サービス例にOpenAI API（Xルート）を追加。制定日と改定日を区別。
5. 旧公式サイトURLを復活させず、サイト自身への相対リンク「./」を維持。
6. 既存のDiscord認証URL（client_id=1504043011884187659 / permissions=8）を変更しない。管理者権限が必要なことを導入案内に明記。
7. HTMLとCSSを一体として整理。外部JavaScript・外部フォント・実装未確認のバックエンド機能は追加しない。
8. HTMLに埋め込まれた元画像、利用規約、免責事項、運営者情報を維持。
9. Xの画像生成等は実装構想・mockテスト通過であり、本番API/Discord実送信は未確認であることを明示。

【次セッションでそのまま使用するプロンプト】
GitHub連携で 1chigoMilk/1chigoMilk.github.io の main ブランチから Ch1llTimeBotOfficialSite/index.html と同じフォルダのREADME.txt、仕様書_V26.11.13.1728.txt、作業報告書_V26.11.13.1728.txtを実取得してください。前回のサイト全面改修の基準コミットは d54d0ed0c9afc4f13e0877ff3c66609cb247031b ですが、必ずその時点の最新HEADとSHAを先に確認してください。既存の完全HTMLとWebP data URI画像、11セクション、FAQ、利用規約・プライバシーポリシー、Discord導入リンク、運営者名（いちごみるく）を失わず、ユーザーが指示した改善を根本的・一貫した設計として実装してください。更新は元の Ch1llTimeBotOfficialSite/index.html に対する完全な内容置換を基本とし、ファイル名を変えず、公開を保証する前にGitHub Pagesの設定と実URLを別途確認してください。HTMLタグ、ID・アンカーリンク、CSS、モバイル表示、外部リンク、秘密情報の混入、法的説明の保持を検証してください。変更のたびに最新の仕様書・報告書・引継ぎ内容を更新してください。

【検証記録】
・GitHub main の更新後HTMLを再取得し、blob SHA=2b4db11a0e71bc744d69675de274efe075a41029を照合。
・HTMLのタグ対応エラー 0、未閉鎖タグ 0。
・ページ内リンク34件、リンク切れ0、ID重複0。
・CSS波括弧の整合PASS。
・メイン画像、規約6項目、Discord招待リンク5件の存在を確認。
・サイトの本番描画、iPhoneの実機表示、GitHub Pagesデプロイ状態および公開URLのHTTP疎通は未実施。
・Bot本体の稼働状態はこのサイト改修の対象外。外部APIの本番成功は保証しない。
