---
title: accessreview リソースの種類
description: 'Azure AD access レビュー機能では、は`accessReview`アクセスレビューを表します。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2cb5d32a8dcc6b12330aca6e831a8ab2083759df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544112"
---
# <a name="accessreview-resource-type"></a>accessreview リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](accessreviews-root.md)機能では、は`accessReview`アクセスレビューを表します。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[accessreview を取得する](../api/accessreview-get.md) |   [accessreview](accessreview.md) |   特定の id を持つアクセスレビューを取得します。 |
|[accessreview を作成する](../api/accessreview-create.md) | [accessreview](accessreview.md) |   新しい accessreview を作成します。 |
|[accessreview の削除](../api/accessreview-delete.md) | なし。   | accessreview を削除します。 |
|[accessreview を更新する](../api/accessreview-update.md) | [accessreview](accessreview.md) | accessreview を更新します。 |
|[accessreview レビュー担当者のリスト](../api/accessreview-listreviewers.md) |      [useridentity](useridentity.md)コレクション| accessreview のレビュー担当者を取得します。 |
|[accessreview レビュー担当者を追加する](../api/accessreview-addreviewer.md) |      なし。   |   閲覧者を accessreview に追加します。 |
|[accessreview レビュー担当者を削除する](../api/accessreview-removereviewer.md) | なし。  |   accessreview からレビュー担当者を削除します。 |
|[accessreview に関する決定事項を一覧表示する](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)コレクション| accessreview の決定事項を取得します。|
|[自分の accessreview の決定事項を一覧表示する](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)コレクション| レビュー担当者として、accessreview の決定事項を取得します。|
|[access レビュー通知の送信](../api/accessreview-sendreminder.md) |        なし。   |   accessreview のレビュー担当者に通知を送信します。 |
|[accessreview を停止する](../api/accessreview-stop.md) |     なし。   |   accessreview を停止します。 |
|[accessreview の決定をリセットする](../api/accessreview-reset.md) |     なし。   |   進行中の accessreview で意思決定をリセットします。|
|[accessreview の決定を適用する](../api/accessreview-apply.md) |     なし。   |   完了した accessreview から決定を適用します。|

## <a name="permissions"></a>アクセス許可

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | accessreview を参照してください。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | アクセスレビューのフィーチャーによって割り当てられた一意の識別子。 |
| `displayName`             |`String`                                                        | アクセスレビュー名。 作成時に必要です。 |
| `startDateTime`           |`DateTimeOffset`                                                | レビューが開始される予定の日時。  これは、将来の日付になる可能性があります。  作成時に必要です。 |
| `endDateTime`             |`DateTimeOffset`                                                | レビューが終了する予定の日時。 これは、開始日よりも1日以上後でなければなりません。  作成時に必要です。 |
| `status`                  |`String`                                                        | この読み取り専用フィールドは、accessreview の状態を指定します。 一般的な状態に`Initializing`は`NotStarted`、 `Starting``InProgress` `Completing` `Completed` `AutoReviewing`、、、、、、 `AutoReviewed`、などがあります。 |
| `description`             |`String`                                                        | レビュー担当者に表示する、アクセスレビュー作成者によって提供される説明。 |
| `businessFlowTemplateId`  |`String`                                                        | ビジネスフローテンプレートの識別子。 作成時に必要です。 |
| `reviewerType`            |`String`                                                        | レビュー担当者の関係の種類 (ターゲットオブジェクト、また`self`は`delegated` `entityOwners`のいずれか)。 作成時に必要です。 | 
| `createdBy`               |[userIdentity](useridentity.md)                                 | このレビューを作成したユーザー。 |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | アクセスレビューでアクセス権の割り当てを確認しているオブジェクト。 これは、グループ内のユーザーのメンバーシップを確認したり、アプリケーションへのユーザーの割り当てを確認したりするためのグループであってもかまいません。 作成時に必要です。 | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | accessreview の設定については、以下の「型の定義」を参照してください。 |



## <a name="relationships"></a>リレーションシップ




| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
| `reviewers`               |[useridentity](useridentity.md)コレクション                     | アクセスレビュー reviewerType の種類`delegate`がの場合に、アクセスレビューのレビュー担当者のコレクション。 |
| `decisions`               |[accessReviewDecision](accessreviewdecision.md)コレクション | このアクセスレビューに関する決定事項のコレクション。 |
| `myDecisions`             |[accessReviewDecision](accessreviewdecision.md)コレクション | 呼び出し元がレビュー担当者の場合、呼び出し元に対する決定のコレクション。 |
| `instances`               |[accessreview](accessreview.md)コレクション         | このオブジェクトが定期的なアクセスレビューである場合、access のコレクションは、過去、現在、および今後のインスタンスをレビューします。 |

オブジェクトにこれらのリレーションシップが存在するかどうかは、オブジェクトが1回限りのアクセスレビューであるか、定期的なアクセスレビューの一連であるか、または定期的なアクセスレビューのインスタンスであるかに応じて異なります。

| シナリオ | レビュー担当者がいますか? | 決定事項と mydecisions はありますか? | インスタンスがあるかどうか |
|:---------|:---------------|:---------------|:---------------|
|ワンタイムアクセスのレビュー|はい | はい (開始した後) | いいえ |
| 定期的なアクセスのレビュー | はい | いいえ | はい |
| 定期的なアクセスレビューのインスタンス | はい | はい (開始した後) | いいえ |

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

## <a name="the-accessreviewsettings-type"></a>accessReviewSettings の種類

は`accessReviewSettings` 、アクセスレビューを作成するときの追加の設定を提供し、アクセスレビューを開始するときの機能の動作を制御します。  この型には、次のプロパティがあります。 

| プロパティ                     | 型                      | 説明 |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | レビュー担当者にメールを送信するかどうか、およびレビュー作成者を有効にするかどうかを示すフラグ。                |
| `remindersEnabled`|`Boolean`       | レビュー担当者に電子メールを送信することが有効かどうかを示すフラグ。       |
| `justificationRequiredOnApproval`|`Boolean` | レビュー担当者がアクセスをレビューする際に理由を指定する必要があるかどうかを示すフラグ。|
| `activityDurationInDays`|`Int64` | ユーザーアクティビティがレビューアーに表示される日数。 |
| `autoReviewEnabled`|`Boolean` | レビュー担当者が自動適用で使用するように指定されていない場合に、機能が決定を設定するかどうかを指定するフラグが有効になります。 |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | 次に示すように、機能によってレビューの決定を設定する方法の詳細設定 (自動適用で使用)。 |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | 定期的なパターンの詳細設定。以下に説明します。 |
| `autoApplyReviewResultsEnabled`|`Boolean` | 自動適用機能を使用して、ターゲットオブジェクトのアクセスリソースを自動的に変更するかどうかを示すフラグが有効になっていることを示します。  有効になっていない場合、ユーザーはレビューが完了した後、アクセスレビューを適用する必要があります。 |
| `accessRecommendationsEnabled`|`Boolean` | レビュー担当者におすすめ候補を表示するかどうかを示すフラグ。 |



## <a name="the-autoreviewsettings-type"></a>autoreviewsettings の種類

は`autoReviewSettings` 、アクセスレビューの設定内に埋め込まれ、アクセスレビューが完了したときの機能の動作を指定します。  この型には、 `notReviewedResult`1 つのプロパティがあります。

| プロパティ                     | 型     | 説明                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | `Approve`、`Deny`、`Recommendation` のいずれかでなければなりません。 |


## <a name="the-accessreviewrecurrencesettings-type"></a>accessReviewRecurrenceSettings の種類

は`accessReviewRecurrenceSettings` 、アクセスレビューの設定内に埋め込まれており、定期的にアクセスレビューが繰り返されることを指定します。  この型には、次のプロパティがあります。

| プロパティ                     | 型                                                                                                          | 説明 |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | 繰り返し間隔。、、、、または`onetime` `annual`の`weekly` `monthly` `quarterly`いずれかである必要があります。                                                                   |
| `recurrenceEndType`|`String` | 定期的なアイテムの終了方法。 その場合は`Never`、定期的なアイテムの明示的な終了はありません。 その場合、 `endBy`定期的なパターンは特定の日付に終了します。 含まれて`occurrences`いる場合は、レビューの`recurrentCount`インスタンスが完了した後に series が終了します。 |
| `durationInDays`|`Int32`     | 定期的なアイテムの期間 (日単位)。                                                                              |
| `recurrenceCount`|`Int32`    | 繰り返しの数 (の`recurrenceEndType`値が`occurrences`である場合)、そうでない場合は0。                                                        |



<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
