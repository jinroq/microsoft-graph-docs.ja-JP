---
title: accessReviewDecision リソースの種類
description: Azure AD にアクセス確認機能を`accessReviewDecision`、Azure AD アクセス確認意思決定の特定のエンティティへのアクセスを表します。  アクセス レビューの場合、または定期的なアクセス確認のインスタンスの中であり、1 つ`accessReviewDecision`確認済みのユーザー 1 人あたり。  などの 2 つのゲストと 1 つ、ゲスト、メンバー、および、アクセス レビュー来園者のグループがある場合は、そのグループのアクセス確認意思決定の 2 つのオブジェクトがありますし。  校閲者が自分の意思決定を変更または別の校閲者が、それらをオーバーライドする場合、`accessReviewDecision`を更新します。
localization_priority: Normal
ms.openlocfilehash: 208337f3427fad65499b400dee769d379c38dcb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870050"
---
# <a name="accessreviewdecision-resource-type"></a>accessReviewDecision リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure AD[アクセスの確認](accessreviews-root.md)機能で、 `accessReviewDecision` 、Azure AD アクセス確認意思決定の特定のエンティティへのアクセスを表します。  アクセス レビューの場合、または定期的なアクセス確認のインスタンスの中であり、1 つ`accessReviewDecision`確認済みのユーザー 1 人あたり。  などの 2 つのゲストと 1 つ、ゲスト、メンバー、および、アクセス レビュー来園者のグループがある場合は、そのグループのアクセス確認意思決定の 2 つのオブジェクトがありますし。  校閲者が自分の意思決定を変更または別の校閲者が、それらをオーバーライドする場合、`accessReviewDecision`を更新します。


## <a name="methods"></a>メソッド

なし  この型のオブジェクトが自動的に作成機能とアクセス確認の初期化、削除することはできません。  それらは、[意思決定](../api/accessreview-listdecisions.md)と[mydecisions](../api/accessreview-listmydecisions.md)の関係を使用して、アクセスの確認から取得できます。

## <a name="properties"></a>プロパティ

次の表は、この型のオブジェクトの基本プロパティを示しています。 

| プロパティ                        | 種類                         | 説明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | アクセス レビュー内での意思決定の id です。                                                                                     |
| `accessReviewId`                |`String`                      | アクセス レビューの機能によって生成された id です。                                                                                       |
| `reviewedBy`                    |[割り当てられていません](useridentity.md)| 校閲者の id です。                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | 日付と時刻の最新のレビューにアクセス権が指定されました。                                                                         |
| `reviewResult`                  |`String`                      | レビューの結果です。                                                                                    |
| `justification`                 |`String`                      | 校閲者のビジネス ・ ジャスティフィケーションを提供された場合。                                                                         |
| `appliedBy`                     |[割り当てられていません](useridentity.md)| レビューの完了時、結果を手動で適用されていた場合、意思決定を適用したユーザーのユーザー id です。                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | 日付と時刻確認の意思決定が適用されています。                                                          |
| `applyResult`                   |`String`                      | いずれかの意思決定を適用した結果`NotApplied`、 `Success`、 `Failed`、`NotFound`または`NotSupported`。                      |
| `accessRecommendation`          |`String`                      | 機能で生成された推奨事項のいずれかの校閲者に示すように`Approve`、`Deny`または`NotAvailable`。 |


さらに、追加のプロパティが決定されているアクセス権を持つオブジェクトのオブジェクトの種類によって表示されます。  たとえば、アクセス確認の意思決定が特定のユーザーのグループ メンバーシップ、またはアプリケーションへのアクセスの場合は、これらのプロパティを使用した可能性があるかのアクセスを削除するユーザーが識別されます。

| プロパティ                        | 種類                         | 説明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | アクセス権が確認されたユーザーの id です。                                                                                    |
| `userDisplayName`                            |`String`                      | アクセス権が確認されたユーザーの表示名。                                                                                     |
| `userPrincipalName`                            |`String`                      | アクセス権が確認されたユーザーのユーザー プリンシパル名です。                                                                                     |



## <a name="relationships"></a>リレーションシップ

なし。  この型のオブジェクトは、 [accessReview](accessreview.md)オブジェクトの[mydecisions](../api/accessreview-listmydecisions.md)の[意思決定](../api/accessreview-listdecisions.md)との関係を使用してアクセス確認から取得できます。

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[リストの accessReview の決定](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)コレクション| AccessReview の決定を取得します。|
|[マイ accessReview の決定事項を表示します。](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)コレクション| 参照者、accessReview の自分の意思決定を取得します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
