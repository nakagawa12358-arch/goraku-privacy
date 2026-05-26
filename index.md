# 碁楽（Goraku）プライバシーポリシー

最終更新日: 2026年5月27日

碁楽（以下「本アプリ」といいます）は、ユーザーのプライバシーを尊重し、個人情報を慎重に取り扱います。本ポリシーは本アプリが取り扱う情報の内容と、その用途を説明するものです。

## 1. 取得する情報

### 1.1 音声データ（マイク・音声認識）
本アプリは音声入力で着手位置を指定する機能を提供します。
- マイクおよび音声認識の利用は、ユーザーが音声入力ボタンをタップした時にのみ動作します。
- 取得した音声は Apple の音声認識サービス（SFSpeechRecognizer）に送信され、テキストに変換されます。Apple のプライバシーポリシーに従って処理されます。
- 本アプリ自体は音声データを保存しません。

### 1.2 匿名ユーザーID
オンライン対局機能を利用する場合、Firebase Authentication（Google）が匿名のユーザーIDを発行します。
- 個人を特定する情報（メールアドレス、氏名等）は一切含まれません。
- アプリを削除すると匿名IDも無効になります。

### 1.3 対局データ・チャットメッセージ
オンライン対局中、以下のデータが Firebase Realtime Database に一時的に保存されます。
- ルームコード、着手情報、対局者の手番状態
- 対局相手と交わしたチャットメッセージ
- これらのデータは対局参加者間で同期するためのものであり、対局終了から一定期間後に自動的に削除されます。

### 1.4 顔データ（カメラ）
本アプリには、画面をタップできない方のための任意のアクセシビリティ機能「まばたきで着手」があります。この機能を**オンにした場合に限り**、端末のフロントカメラ（TrueDepth）と Apple の ARKit を使用して、まばたき（目の開閉の度合い）をリアルタイムに検出します。
- **取得する情報**: まばたき判定に用いる ARKit の数値（目の開閉の度合い）のみです。顔の画像・写真・3D形状・本人を識別する情報は一切取得しません。
- **利用目的**: まばたきを碁盤上の着手操作（列・行の選択と着手の確定）に変換するためだけに使用します。
- **保存**: 顔データは端末内でリアルタイムに処理するのみで、保存しません。
- **送信・共有**: いかなる顔データもデバイス外へ送信せず、サーバー（Firebase 等）にも送らず、第三者と共有しません。
- **保持期間**: 保持しません（処理後ただちに破棄されます）。
- 「まばたきで着手」をオフにしている間はカメラを使用しません。

### Face Data (Camera) — English
The app includes an optional accessibility feature, "Blink to Play," for users who cannot tap the screen. **Only when this feature is turned on**, the app uses the device's front (TrueDepth) camera together with Apple's ARKit to detect blinks (the degree to which the eyes are open or closed) in real time.
- **Information accessed**: Only ARKit blink values (eye open/close coefficients). The app does **not** capture facial images, photos, 3D face geometry, or any data that identifies the user.
- **Purpose**: Solely to convert blinks into Go move input (selecting a column/row and placing a stone).
- **Storage**: Processed in real time on-device only; never stored.
- **Sharing/Transmission**: No face data ever leaves the device; it is not sent to any server (including Firebase) and is not shared with any third party.
- **Retention**: Not retained; discarded immediately after processing. The camera is not used while the feature is off.

## 2. 取得しない情報
本アプリは以下の情報を取得・収集しません。
- 氏名、メールアドレス、電話番号などの個人情報
- 位置情報、連絡先、写真、カレンダー
- 広告識別子（IDFA）
- アプリ利用状況の分析データ（アナリティクス）

## 3. 第三者への提供
本アプリは取得した情報を広告目的・販売目的で第三者に提供することはありません。
ただし、以下のサービスに対してのみ機能提供のために必要なデータを送信します。
- **Apple 音声認識サービス**: 音声データのテキスト変換
- **Firebase（Google）**: オンライン対局・匿名認証

## 4. 子どもの利用について
本アプリは年齢制限 4+ で提供されており、お子様でも安全にお使いいただけます。個人情報の収集は行っておりません。

## 5. ポリシーの変更
本ポリシーは予告なく変更される場合があります。重要な変更がある場合はアプリ内またはこのページでお知らせします。

## 6. お問い合わせ
本ポリシーに関するご質問は以下までご連絡ください。

メール: nakagawa12358@gmail.com
