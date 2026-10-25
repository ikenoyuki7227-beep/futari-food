ふたりの食費 セットアップ

1. Firebase Console (https://console.firebase.google.com/) でプロジェクトを作成。
2. 「構築 > Authentication > Sign-in method」で「メール/パスワード」を有効化。
3. 「構築 > Firestore Database」でデータベースを作成（本番環境モード推奨）。
4. Firestore > ルールに firestore.rules の全文を貼り付けて「公開」。
5. プロジェクト設定 > マイアプリ > ウェブアプリを登録し、firebaseConfigのJSONをコピー。
6. GitHubで新しい公開リポジトリを作り、index.html, manifest.webmanifest, icon.png をアップロード。
7. Settings > Pages > Deploy from a branch > main / (root) > Save。表示されたURLをSafariで開く。
8. Firebase接続情報はindex.htmlに組み込み済み。設定JSONの入力は不要。
9. 「初めて使う：家計を作成」で共通メールアドレスとパスワードを登録。
10. 設定タブで予算・週開始曜日・利用開始日を設定。
11. 2台目も同じURLを開き、同じメールアドレスとパスワードでログイン。
12. iPhoneのSafari共有メニュー > ホーム画面に追加。

重要:
・夫婦は同じログインアカウントを共有する設計です。Firebaseのメール/パスワード認証で保護されます。
・Firebaseの設定JSONは秘密鍵ではありませんが、Firestoreルールの設定は必須です。
・夫婦それぞれの端末で「この端末の入力者名」を設定してください。
・履歴の削除はできますが、編集機能はありません。修正時は削除して再登録してください。
・節約額には進行中の週の未使用額も含まれます。
・週予算や開始曜日の変更は過去の週の表示にも反映されます。
・Firestore無料枠内での運用を想定していますが、利用状況によって課金や制限が発生する場合があります。
