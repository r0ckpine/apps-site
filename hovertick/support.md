# Support / サポート — HoverTick

## 日本語

HoverTickは、ライブアクティビティ(Dynamic Islandとロック画面)とピクチャインピクチャに対応したタイマーアプリです。

### お問い合わせ

**メール**: hovertick.support@gmail.com

### よくある質問 (FAQ)

**Q. ライブアクティビティ(ロック画面表示)が表示されません**

A. iPhoneの設定アプリ →「HoverTick」→「ライブアクティビティ」がオンになっているかご確認ください。

**Q. ピクチャインピクチャが使えません**

A. ピクチャインピクチャはHoverTick Proの機能です。ほかのアプリでピクチャインピクチャを使用中の場合は、同時に表示できないことがあります。

**Q. HoverTick Proを家族と共有できますか？**

A. はい。HoverTick Proは買い切りで、ファミリー共有に対応しています。ファミリー共有グループのメンバーは追加料金なしで利用できます。家族のデバイスでロックが解除されない場合は、そのデバイスで「購入を復元」をお試しください。

**Q. 購入した内容を復元したい**

A. アプリ内の「設定」→「HoverTick Pro」→「購入を復元」をお試しください(HoverTick Proの購入画面にもあります)。購入時と同じApple Accountでサインインしている必要があります。同じApple Accountであれば、iPhoneとiPadの両方で利用できます。

### セッション履歴について

タイマー、ストップウォッチ、シーケンスの記録が「履歴」タブに自動で保存されます。履歴はお使いの端末内にのみ保存されます。

#### 記録の単位

- **タイマーとストップウォッチ**: 1回の計測ごとに1件記録されます。ラベルは開始前と一時停止中に変更できますが、終了時のラベルのみが記録されます。
- **シーケンス**: ステップごとに1件記録されます。ステップはスキップやステップ間の移動ができるため、各ステップが終わった時点でそれぞれ記録されます(シーケンス全体をまとめた記録はありません)。ラベルは「シーケンス名 − ステップ名」になります。

#### 記録される内容

| 項目 | 内容 |
|------|------|
| モード | タイマー / ストップウォッチ / シーケンス |
| ラベル | タイマーとストップウォッチは、文字盤のメニューで選択したラベル(例:「仕事」)。未選択の場合は表示されません。シーケンスは「シーケンス名 − ステップ名」です。 |
| 予定時間 | タイマーは設定した時間、シーケンスはそのステップの時間です。ストップウォッチにはありません。 |
| 実行時間 | 実際に動いていた時間です。**一時停止していた時間は含みません。** 履歴の一覧にはこの時間が表示されます。 |
| 開始・終了時刻 | 実際の時刻です。開始から終了までの間には **一時停止していた時間も含まれます。** 行をタップすると表示されます。 |
| 結果 | 下の表のとおりです。 |

#### 結果の種類

どのモードでも(シーケンスではステップごとに)、同じルールで決まります。

| 結果 | 終了状態 | 終了時刻 |
|------|----------------|----------|
| 完了 | 0に到達 | 0になった時刻 |
| 停止 | **一時停止中に**、リセット、次/前のステップ、「戻る」のいずれかで終了 | 最後に一時停止した時刻 |
| リセット | 動作中にリセット | リセットした時刻 |
| スキップ | シーケンスの動作中に、次/前のステップへ移動 | 操作した時刻 |
| 中断 | シーケンスの動作中に、「戻る」で終了 | 操作した時刻 |

一時停止してから終了した場合は、意図的な終了とみなして「停止」として扱い、動作中にキャンセルした場合とは区別します。

- 「完了」の記録では、実行時間は予定時間と一致します。
- 設定の「ゼロを過ぎてもカウントアップ」(初期設定はオフ)をオンにすると、タイマーは0を過ぎても止まらずにカウントアップを続けます。0を過ぎてから終了した場合、実行時間は設定時間と同一として「停止」または「リセット」で記録されます。

#### 記録されないもの

- 一度も開始していないタイマーのリセット
- 0:00のままのストップウォッチ
- 一度も動かさなかったシーケンスのステップ
- ストップウォッチのラップ(ラップはストップウォッチ画面の「ラップを書き出す」からCSVとして書き出せます)

#### 保存件数

履歴は最大5,000件まで保存されます。それを超えると、古いものから自動的に削除されます。

#### 履歴の見かた

履歴は日ごとにまとめて新しい日から表示され、1日ごとの合計時間も表示されます。行をタップすると、開始・終了時刻などの詳細が開きます。モード、期間(全期間 / 今日 / 今週 / 今月、または任意の期間)、結果、ラベルで絞り込めるほか、新しい順・古い順に並べ替えられます。ラベルの絞り込みには過去の記録で使われたラベルが表示されるため、設定から削除したラベルでも絞り込めます。

#### 書き出しと削除

「選択」で記録を選ぶと、画面下部から次の操作ができます。

- **共有**(Pro): CSVファイル(表計算アプリ向け)と、1件1行のテキスト(メモ・メール・メッセージ向け)のどちらでも共有できます。CSVの列は `mode, label, planned_seconds, actual_seconds, start, end, reason` です(日時はISO 8601形式、結果は英語の固定値)。
- **カレンダーに追加**(Pro): 選んだ記録を1件ずつ予定としてカレンダーに追加します。タイトルはラベル(ラベルなしの場合はモード名)、時間帯は記録の開始・終了時刻で、メモに実行時間と結果が入ります。カレンダーへのアクセスは**書き込み専用**で、既存の予定を読み取ることはありません。終了したセッションを自動でカレンダーに追加する機能はありません。
- **削除**: 確認のうえ、選んだ記録を削除します。無料でご利用いただけます。

### バージョン情報

- 最新バージョン: 1.0.0
- 対応OS: iOS 26.0以降、iPadOS 26.0以降(iPhone、iPad)

---

## English

HoverTick is a timer app with Live Activity (Dynamic Island and Lock Screen) and Picture in Picture support.

### Contact Us

**Email**: hovertick.support@gmail.com

### FAQ

**Q. The Live Activity isn't showing on the Lock Screen**

A. Check that Settings → HoverTick → Live Activities is turned on.

**Q. Picture in Picture doesn't work**

A. Picture in Picture is part of HoverTick Pro. It may not appear while another app is already using Picture in Picture.

**Q. Can my family use HoverTick Pro?**

A. Yes. HoverTick Pro is a one-time purchase with Family Sharing, so members of your Family Sharing group can use it at no extra cost. If it doesn't unlock on a family member's device, tap Restore Purchases on that device.

**Q. How do I restore my purchase?**

A. In the app, go to Settings → HoverTick Pro → Restore Purchases (the button is also on the HoverTick Pro purchase screen). You must be signed in with the same Apple Account used for the original purchase. One purchase works on both iPhone and iPad signed in to that Apple Account.

### About Session History

Timer, stopwatch, and sequence sessions are saved to the History tab automatically. History is stored only on your device.

#### What counts as one record

- **Timer and stopwatch**: one record per session. You can change the label before starting or while paused, but only the label set when the session ends is recorded.
- **Sequence**: one record per step. Steps can be skipped or revisited, so each step is recorded as it ends; there is no record for the sequence as a whole. The label is "sequence name − step name".

#### What is recorded

| Item | Meaning |
|------|---------|
| Mode | Timer / Stopwatch / Sequence |
| Label | For a timer or stopwatch, the label chosen from the menu on the timer face (for example, "Work"). Nothing is shown if no label was chosen. For a sequence, "sequence name − step name". |
| Planned time | The time you set for a timer, or the step's length for a sequence. Stopwatches have none. |
| Running time | How long the timer actually ran. **Paused time is not included.** This is the time shown in the History list. |
| Start and end times | The actual clock times. The span between them **includes paused time**. Tap a row to see them. |
| Outcome | See the table below. |

#### Outcomes

The same rules apply in every mode (and to each step of a sequence).

| Outcome | How it ended | End time |
|---------|--------------|----------|
| Completed | Reached 0 | When it reached 0 |
| Stopped | Ended **while paused**, by Reset, Next/Previous Step, or Back | When it was last paused |
| Reset | Reset while running | When Reset was tapped |
| Skipped | A sequence moved to the next or previous step while running | When the button was tapped |
| Cleared | A sequence was ended with Back while running | When Back was tapped |

Ending a session after pausing it is treated as a deliberate end and recorded as Stopped, separately from cancelling a running timer.

- For a Completed record, the running time matches the planned time.
- With "Count up past zero" turned on in Settings (off by default), a timer keeps counting up after reaching 0 instead of stopping. If you end it after it passes 0, the running time is recorded as exactly the set time, as Stopped or Reset.

#### What is not recorded

- Resetting a timer that was never started
- A stopwatch still at 0:00
- A sequence step that never ran
- Stopwatch laps (you can export them as a CSV with Export Laps on the stopwatch screen)

#### How many records are kept

Up to 5,000 records are kept. Beyond that, the oldest are removed automatically.

#### Browsing history

History is grouped by day, newest day first, with a total for each day. Tap a row to see its start and end times and other details. You can filter by mode, date range (All Time, Today, This Week, This Month, or a custom range), outcome, and label, and sort newest or oldest first. The label filter offers every label used in past records, so you can still filter by a label you've since deleted in Settings.

#### Exporting and deleting

Tap Select and choose records to use the actions at the bottom of the screen:

- **Share** (Pro): share as a CSV file for spreadsheets, or as plain text with one line per record for Notes, Mail, or Messages. The CSV columns are `mode, label, planned_seconds, actual_seconds, start, end, reason` (dates in ISO 8601; the outcome as a fixed English value).
- **Add to Calendar** (Pro): adds each selected record to your calendar as its own event. The title is the label (or the mode name if unlabeled), the event spans the record's start and end times, and the notes include the running time and outcome. Calendar access is **write-only**, so HoverTick never reads your existing events. Finished sessions are never added to your calendar automatically.
- **Delete**: removes the selected records after you confirm. Free for everyone.

### Version Info

- Latest version: 1.0.0
- Requires: iOS 26.0 or later, iPadOS 26.0 or later (iPhone and iPad)
