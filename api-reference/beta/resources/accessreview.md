---
title: accessReview リソースの種類
description: 'Azure AD access レビュー機能では、は`accessReview`アクセスレビューを表します。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4205f0995b0e8c71c8e01991837b4d721ecfaaf7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974571"
---
# <a name="accessreview-resource-type"></a>accessReview リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](accessreviews-root.md)機能では、は`accessReview`アクセスレビューを表します。  


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview を取得する](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   特定の id を持つアクセスレビューを取得します。 |
|[AccessReview を作成する](../api/accessreview-create.md) | [accessReview](accessreview.md) |   新しい accessReview を作成します。 |
|[AccessReview の削除](../api/accessreview-delete.md) | なし。   | AccessReview を削除します。 |
|[AccessReview を更新する](../api/accessreview-update.md) | [accessReview](accessreview.md) | AccessReview を更新します。 |
|[AccessReview レビュー担当者のリスト](../api/accessreview-listreviewers.md) |      [Useridentity](useridentity.md)コレクション| AccessReview のレビュー担当者を取得します。 |
|[AccessReview レビュー担当者を追加する](../api/accessreview-addreviewer.md) |      なし。   |   閲覧者を accessReview に追加します。 |
|[AccessReview レビュー担当者を削除する](../api/accessreview-removereviewer.md) | なし。  |   AccessReview からレビュー担当者を削除します。 |
|[AccessReview に関する決定事項を一覧表示する](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)コレクション| AccessReview の決定事項を取得します。|
|[自分の accessReview の決定事項を一覧表示する](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)コレクション| レビュー担当者として、accessReview の決定事項を取得します。|
|[Access レビュー通知の送信](../api/accessreview-sendreminder.md) |        なし。   |   AccessReview のレビュー担当者に通知を送信します。 |
|[AccessReview を停止する](../api/accessreview-stop.md) |     なし。   |   AccessReview を停止します。 |
|[AccessReview の決定をリセットする](../api/accessreview-reset.md) |     なし。   |   進行中の accessReview で意思決定をリセットします。|
|[AccessReview の決定を適用する](../api/accessreview-apply.md) |     なし。   |   完了した accessReview から決定を適用します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | アクセスレビューのフィーチャーによって割り当てられた一意の識別子。 |
| `displayName`             |`String`                                                        | アクセスレビュー名。 作成時に必要です。 |
| `startDateTime`           |`DateTimeOffset`                                                | レビューが開始される予定の日時。  これは、将来の日付になる可能性があります。  作成時に必要です。 |
| `endDateTime`             |`DateTimeOffset`                                                | レビューが終了する予定の日時。 これは、開始日よりも1日以上後でなければなりません。  作成時に必要です。 |
| `status`                  |`String`                                                        | この読み取り専用フィールドは、accessReview の状態を指定します。 一般的な状態に`Initializing`は`NotStarted`、 `Starting``InProgress` `Completing` `Completed` `AutoReviewing`、、、、、、 `AutoReviewed`、などがあります。 |
| `description`             |`String`                                                        | レビュー担当者に表示する、アクセスレビュー作成者によって提供される説明。 |
| `businessFlowTemplateId`  |`String`                                                        | ビジネスフローテンプレートの識別子。 作成時に必要です。 |
| `reviewerType`            |`String`                                                        | レビュー担当者の関係の種類 (ターゲットオブジェクト、また`self`は`delegated` `entityOwners`のいずれか)。 作成時に必要です。 | 
| `createdBy`               |[userIdentity](useridentity.md)                                 | このレビューを作成したユーザー。 |
| `reviewedEntity`          |[identity](identity.md)                                      | アクセスレビューでアクセス権の割り当てを確認しているオブジェクト。 これは、グループ内のユーザーのメンバーシップを確認したり、アプリケーションへのユーザーの割り当てを確認したりするためのグループであってもかまいません。 作成時に必要です。 | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | AccessReview の設定については、以下の「型の定義」を参照してください。 |



## <a name="relationships"></a>リレーションシップ




| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
| `reviewers`               |[Useridentity](useridentity.md)コレクション                     | アクセスレビュー reviewerType の種類`delegate`がの場合に、アクセスレビューのレビュー担当者のコレクション。 |
| `decisions`               |[accessReviewDecision](accessreviewdecision.md)コレクション | このアクセスレビューに関する決定事項のコレクション。 |
| `myDecisions`             |[accessReviewDecision](accessreviewdecision.md)コレクション | 呼び出し元がレビュー担当者の場合、呼び出し元に対する決定のコレクション。 |
| `instances`               |[Accessreview](accessreview.md)コレクション         | このオブジェクトが定期的なアクセスレビューである場合、access のコレクションは、過去、現在、および今後のインスタンスをレビューします。 |

オブジェクトにこれらのリレーションシップが存在するかどうかは、オブジェクトが1回限りのアクセスレビューであるか、定期的なアクセスレビューの一連であるか、または定期的なアクセスレビューのインスタンスであるかに応じて異なります。

| シナリオ | レビュー担当者がいますか? | 決定事項と myDecisions はありますか? | インスタンスがあるかどうか |
|:---------|:---------------|:---------------|:---------------|
|ワンタイムアクセスのレビュー|はい | はい (開始した後) | いいえ |
| 定期的なアクセスのレビュー | はい | いいえ | はい |
| 定期的なアクセスレビューのインスタンス | はい | はい (開始した後) | いいえ |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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

## <a name="the-accessreviewsettings-type"></a>AccessReviewSettings の種類

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

## <a name="the-autoreviewsettings-type"></a>AutoReviewSettings の種類

は`autoReviewSettings` 、アクセスレビューの設定内に埋め込まれ、アクセスレビューが完了したときの機能の動作を指定します。  この型には、 `notReviewedResult`1 つのプロパティがあります。

| プロパティ                     | 型     | 説明                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | `Approve`、`Deny`、`Recommendation` のいずれかでなければなりません。 |


## <a name="the-accessreviewrecurrencesettings-type"></a>AccessReviewRecurrenceSettings の種類

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
  "suppressions": []
}
-->
