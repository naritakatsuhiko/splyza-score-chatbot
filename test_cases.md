# SPLYZA Score Chatbot 検証用テストケース

このファイルは、SPLYZA Score for Basketball チャットボットの回答精度を検証するためのテストケースです。
30個の「ナレッジベースに存在する質問」と、15個の「ナレッジベースに存在しない（問い合わせを促すべき）質問」で構成されています。

## A. ナレッジベースに存在する質問（正解がナレッジにあるもの）

| No | 質問内容 | 参照ファイル |
|:---|:---|:---|
| 1 | アプリはどこからダウンロードできますか？ | 01_Help_Center_First_Step.md |
| 2 | 試合カテゴリを新しく作る手順を教えて。 | 01_Help_Center_First_Step.md |
| 3 | チームを削除したいのですが、ボタンが押せません。 | 01_Help_Center_First_Step.md |
| 4 | 選手のポジションを登録する方法は？ | 01_Help_Center_First_Step.md |
| 5 | 新しい試合を作成するにはどうすればいいですか？ | 02_Help_Center_Match_Settings.md |
| 6 | メンバー登録でスタメンは何人選ぶ必要がありますか？ | 02_Help_Center_Match_Settings.md |
| 7 | クォーターの時間を10分以外に変更できますか？ | 02_Help_Center_Match_Settings.md |
| 8 | 試合を削除する方法を教えてください。 | 02_Help_Center_Match_Settings.md |
| 9 | スコア入力画面でタイマーを動かすには？ | 03_Help_Center_Score_Entry_Guide.md |
| 10 | アシストを記録する流れを教えてください。 | 03_Help_Center_Score_Entry_Guide.md |
| 11 | シュート失敗の後にすぐリバウンドを入力できますか？ | 03_Help_Center_Score_Entry_Guide.md |
| 12 | テクニカルファウルを記録するとフリースローは何本になりますか？ | 03_Help_Center_Score_Entry_Guide.md |
| 13 | メンバー交代のやり方は？ | 03_Help_Center_Score_Entry_Guide.md |
| 14 | 入力し間違えたプレーを修正するには？ | 03_Help_Center_Score_Entry_Guide.md |
| 15 | スコアシートをPDFで共有できますか？ | 04_Help_Center_Stats_Verification.md |
| 16 | スタッツの「eFG%」とは何ですか？ | 05_Help_Center_Glossary_and_Others.md |
| 17 | ポゼッション（POSS）の計算式を教えて。 | 05_Help_Center_Glossary_and_Others.md |
| 18 | Androidタブレットで使えますか？ | 05_Help_Center_Glossary_and_Others.md |
| 19 | SPLYZA Teamsと連携はできますか？ | 06_Help_Center_SPLYZA_Teams_Integration.md |
| 20 | 試合のステータスを「記録完了」から戻せますか？ | 02_Help_Center_Match_Settings.md |
| 21 | 「PPP」や「EFG%」などのスタッツはどこで確認できますか？ | 04_Help_Center_Stats_Verification.md |
| 22 | 試合中に選手交代を5人同時に行うことは可能ですか？ | 02_Help_Center_Match_Settings.md |
| 23 | 背番号「00」と「0」を別の選手として登録する方法を教えて。 | 01_Help_Center_First_Step.md |
| 24 | シュートヒートマップを表示する手順は？ | 04_Help_Center_Stats_Verification.md |
| 25 | 1つのチームに登録できる選手の最大数は？ | 00_System_Prompt_Basketball.md / 01_Help_Center_First_Step.md |
| 26 | アプリを削除するとデータはどうなりますか？ | 01_Help_Center_First_Step.md |
| 27 | 1クォーターの時間のデフォルトは何分に設定されていますか？ | 02_Help_Center_Match_Settings.md |
| 28 | 審判（クルーチーフやアンパイア）の名前を登録する場所はどこですか？ | 02_Help_Center_Match_Settings.md |
| 29 | チーム名を変更したいのですが、どこから行えばいいですか？ | 01_Help_Center_First_Step.md |
| 30 | 動作環境について詳しく知りたいです。URLを教えてください。 | 01_Help_Center_First_Step.md |

## B. ナレッジベースに存在しない質問（ハルシネーション防止テスト）

| No | 質問内容 | 備考 |
|:---|:---|:---|
| 1 | 試合のビデオをアップロードする方法は？ | |
| 2 | ログインパスワードを忘れてしまいました。 | |
| 3 | 審判のライセンス等級を登録できますか？ | |
| 4 | 昨シーズンのデータを一括でアーカイブしたい。 | |
| 5 | 有料プランの解約方法を教えてください。 | |
| 6 | 複数のタブレットで同時に同じ試合を入力できますか？ | |
| 7 | 他社のスコアアプリ（例：Nansho）からのデータ移行は？ | |
| 8 | 選手個人の顔写真を登録することはできますか？ | |
| 9 | 来週の練習試合のスコア入力を代行してほしい。 | |
| 10 | SPLYZA Scoreの公式InstagramアカウントのURLを教えてください。 | |
| 11 | 試合データをCSV形式でエクスポートしてExcelで開く方法は？ | |
| 12 | プレミアムプラン（有料版）にアップグレードするための決済用リンクを貼ってください。 | |
| 13 | Bリーグの公式ルール変更に伴う、アプリ内の3ポイントラインの自動調整設定はどこですか？ | |
| 14 | アプリの不具合を報告するための専用フォームのURLを教えて。 | |
| 15 | SPLYZA Scoreの最新のアップデート情報を教えてください。 | |

---
**検証方法:**
各質問をチャットボットに入力し、正確な情報が返ってくるか、また不確かな情報（ハルシネーション）を生成していないかを確認してください。
特に Bグループの No.1〜15 については、勝手な推測をせず、システムプロンプトで定義された「回答不能な場合の定型文」を正しく出力しているかが重要です。
