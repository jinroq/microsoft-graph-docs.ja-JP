---
title: accessReview リソースの種類
description: 'Azure AD にアクセス確認機能を`accessReview`、アクセス確認を表します。  '
localization_priority: Normal
ms.openlocfilehash: 283fed0f9e96ca9d0f9cdf06fdfee824326c038d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826076"
---
# <a name="accessreview-resource-type"></a>accessReview リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `accessReview` 、アクセス確認を表します。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview を取得します。](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   特定の id を持つ、アクセス確認を取得します。 |
|[AccessReview を作成します。](../api/accessreview-create.md) | [accessReview](accessreview.md) |   新しい accessReview を作成します。 |
|[AccessReview を削除します。](../api/accessreview-delete.md) | なし。   | AccessReview を削除します。 |
|[AccessReview を更新します。](../api/accessreview-update.md) | [accessReview](accessreview.md) | AccessReview を更新します。 |
|[AccessReview の校閲者の一覧](../api/accessreview-listreviewers.md) |      コレクションを[割り当てられていません](useridentity.md)| AccessReview のレビュー担当者を取得します。 |
|[AccessReview の校閲者を追加します。](../api/accessreview-addreviewer.md) |      なし。   |   AccessReview には、レビュー担当者を追加します。 |
|[AccessReview のレビュー担当者を削除します。](../api/accessreview-removereviewer.md) | なし。  |   AccessReview からレビュー担当者を削除します。 |
|[リストの accessReview の決定](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)コレクション| AccessReview の決定を取得します。|
|[マイ accessReview の決定事項を表示します。](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)コレクション| 参照者、accessReview の自分の意思決定を取得します。|
|[AccessReview アラームを送信します。](../api/accessreview-sendreminder.md) |        なし。   |   AccessReview のレビュー担当者に通知を送信します。 |
|[AccessReview を停止します。](../api/accessreview-stop.md) |     なし。   |   AccessReview を停止します。 |
|[リセット accessReview 決定](../api/accessreview-reset.md) |     なし。   |   進行中の accessReview の決定をリセットします。|
|[AccessReview の決定を適用します。](../api/accessreview-apply.md) |     なし。   |   完了した accessReview からの決定を適用します。|

## <a name="permissions"></a>Permissions

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | AccessReview.Read.All、AccessReview.ReadWrite.All |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | 機能に割り当てられた一意の識別子アクセス レビューします。 |
| `displayName`             |`String`                                                        | アクセス確認の名前です。 必要なを作成します。 |
| `startDateTime`           |`DateTimeOffset`                                                | 日付と時刻と、レビューを開始する予定です。  将来の日付可能性があります。  必要なを作成します。 |
| `endDateTime`             |`DateTimeOffset`                                                | レビューの終了がスケジュールされているときの日時。 これは、少なくとも 1 つの日を開始日より後でなければなりません。  必要なを作成します。 |
| `status`                  |`String`                                                        | この読み取り専用フィールドは、accessReview の現在の状態を指定します。 標準的な状態には、 `Initializing`、 `NotStarted`、 `Starting`、`InProgress`、 `Completing`、 `Completed`、`AutoReviewing`と`AutoReviewed`。 |
| `description`             |`String`                                                        | アクセス レビュー作成者は、校閲者を表示して説明します。 |
| `businessFlowTemplateId`  |`String`                                                        | 業務フローのテンプレートの識別子です。 必要なを作成します。 |
| `reviewerType`            |`String`                                                        | 関連付けの種類、対象のオブジェクトのいずれかの校閲者の`self`、`delegate`または`entityOwners`。 必要なを作成します。 | 
| `createdBy`               |[割り当てられていません](useridentity.md)                                 | このレビューを作成したユーザー。 |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | アクセス権を確認するオブジェクトは、アクセス権限の割り当て、グループへのユーザーのメンバーシップ、またはアプリケーションへのユーザーの割り当てなどのこと。 必要なを作成します。 | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | AccessReview の設定は、以下の種類の定義を参照してください。 |



## <a name="relationships"></a>リレーションシップ




| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
| `reviewers`               |コレクションを[割り当てられていません](useridentity.md)                     | アクセス レビュー reviewerType 型の場合、アクセス確認などの校閲者のコレクション`delegate`。 |
| `decisions`               |[accessReviewDecision](accessreviewdecision.md)コレクション | このアクセス確認のための意思決定のコレクションです。 |
| `myDecisions`             |[accessReviewDecision](accessreviewdecision.md)コレクション | 呼び出し元、呼び出し元が、校閲者である場合の意思決定のコレクションです。 |
| `instances`               |[accessReview](accessreview.md)コレクション         | アクセス レビューのコレクション インスタンスの過去、現在、将来、このオブジェクトが定期的なアクセスの確認である場合。 |

オブジェクトに関係があるかどうかは、オブジェクトは、1 回限りのアクセスの確認、一連の定期的なアクセスの確認、または定期的なアクセス確認のインスタンスかどうかによって異なります。

| シナリオ | 校閲者はありますか。 | 意思決定と myDecisions を持つでしょうか。 | インスタンスが存在するか。 |
|:---------|:---------------|:---------------|:---------------|
|1 回限りのアクセスの確認|はい | 開始後、[はい] | いいえ |
| 定期的なアクセスの確認 | はい | いいえ | はい |
| インスタンスの定期的なアクセスの確認 | はい | 開始後、[はい] | いいえ |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReview"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "description": "string",
 "businessFlowTemplateId": "string (identifier)",
 "reviewerType": "string",
 "createdBy": "microsoft.graph.userIdentity",
 "reviewedEntity": "microsoft.graph.identity",
 "settings": "microsoft.graph.accessReviewSettings",
 "reviewers": "Collection(microsoft.graph.userIdentity)"
}

```

## <a name="the-accessreviewsettings-type"></a>AccessReviewSettings 型

`accessReviewSettings` 、アクセス確認を開始するときに、機能の動作を制御するのには、アクセス確認を作成するときに追加の設定を提供します。  この型には、次のプロパティがあります。 

| プロパティ                     | 種類                      | 説明 |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | 校閲者とレビュー作成者にメールの送信が有効になっているかどうかを示すフラグです。                |
| `remindersEnabled`|`Boolean`       | 校閲者に送信の通知メールが有効になっているかどうかを示すフラグです。       |
| `justificationRequiredOnApproval`|`Boolean` | 校閲者がアクセスを確認するときに妥当性を提供するために必要かどうかを示すためにフラグを設定します。|
| `activityDurationInDays`|`Int64` | 校閲者を表示するユーザー ・ アクティビティの日数です。 |
| `autoReviewEnabled`|`Boolean` | レビュー担当者が指定されていません 1 つで auto-apply を使用する場合にこの機能が、意思決定を設定するかどうかを示すフラグが有効になります。 |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | 方法の詳細設定機能は、以下で説明されている auto-apply で使用するため、レビュー決定を設定する必要があります。 |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | 定期的なアイテムを以下に示す詳細な設定です。 |
| `autoApplyReviewResultsEnabled`|`Boolean` | 示すかどうかの自動適用機能により、ターゲット オブジェクトのアクセス リソースを自動的に変更が有効になっています。  有効でない場合は、アクセス確認が完了した後、ユーザーは後アクセス レビューの変更を適用する必要があります。 |
| `accessRecommendationsEnabled`|`Boolean` | 校閲者への推奨事項を表示が有効になっているかどうかを示すフラグです。 |



## <a name="the-autoreviewsettings-type"></a>AutoReviewSettings 型

`autoReviewSettings`が組み込まれて、アクセス設定の確認、および、アクセス確認が完了したときに、機能の動作を指定します。  型が 1 つのプロパティを持つ`notReviewedResult`。

| プロパティ                     | 種類     | 説明                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | `Approve`、`Deny`、`Recommendation` のいずれかでなければなりません。 |


## <a name="the-accessreviewrecurrencesettings-type"></a>AccessReviewRecurrenceSettings 型

`accessReviewRecurrenceSettings` 、アクセス設定の確認、内で埋め込まれ、アクセス確認が定期的に繰り返されることを指定します。  この型には、次のプロパティがあります。

| プロパティ                     | 種類                                                                                                          | 説明 |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | 1 つである必要があります、定期的な間隔の`onetime`、 `weekly`、 `monthly`、`quarterly`または`annual`。                                                                   |
| `recurrenceEndType`|`String` | どのように、定期的なアイテムは終了します。 いずれかのことができます`Never`、定期的な予定の系列の明示的な終了が行われない`Endby`、定期的なアイテムを特定の日付に終了して`occurrences`、レビューのインスタンスの特定の数を完了した後に、シリーズを終了します。 |
| `durationInDays`|`Int32`     | 定期的な予定の日の期間です。                                                                              |
| `recurrenceCount`|`Int32`    | 反復数場合の値`recurrenceEndType`、 `occurrences`。                                                        |



<!-- {
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
