---
title: accessReviewDecision リソースの種類
description: Azure AD access レビュー機能では、は`accessReviewDecision`特定のエンティティのアクセスに対する azure ad アクセスレビューの決定を表します。  アクセスレビュー、または定期的なアクセスレビューのインスタンスでは、レビュー対象の`accessReviewDecision`ユーザーごとに1つあります。  たとえば、グループに2人のゲストとゲスト以外のゲストがメンバーとして設定されている場合、そのグループに対してゲストのアクセスレビューが行われると、2つのアクセスレビューの決定オブジェクトがあります。  レビュー担当者が決定を変更した場合、または別の`accessReviewDecision`レビュー担当者がそれを上書きした場合は、が更新されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 034ecbdaa108d0c63378d1c00136f0415019b262
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657743"
---
# <a name="accessreviewdecision-resource-type"></a>accessReviewDecision リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](accessreviews-root.md)機能では、は`accessReviewDecision`特定のエンティティのアクセスに対する azure ad アクセスレビューの決定を表します。  アクセスレビュー、または定期的なアクセスレビューのインスタンスでは、レビュー対象の`accessReviewDecision`ユーザーごとに1つあります。  たとえば、グループに2人のゲストとゲスト以外のゲストがメンバーとして設定されている場合、そのグループに対してゲストのアクセスレビューが行われると、2つのアクセスレビューの決定オブジェクトがあります。  レビュー担当者が決定を変更した場合、または別の`accessReviewDecision`レビュー担当者がそれを上書きした場合は、が更新されます。


## <a name="methods"></a>メソッド

なし。  この種類のオブジェクトは、アクセスレビューの初期化時にフィーチャーによって自動的に作成され、削除することはできません。  これらは、[決定](../api/accessreview-listdecisions.md)と[mydecisions](../api/accessreview-listmydecisions.md)の関係を使用して、アクセスレビューから取得できます。

## <a name="properties"></a>プロパティ

この表は、この種類のオブジェクトの基本プロパティを示しています。 

| プロパティ                        | 型                         | 説明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | アクセスレビュー内での決定の id。                                                                                     |
| `accessReviewId`                |`String`                      | アクセスレビューのフィーチャー生成された id。                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| レビュー担当者の id。                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | このアクセス権に関する最新のレビューが提供された日付と時刻。                                                                         |
| `reviewResult`                  |`String`                      | レビューの結果。                                                                                    |
| `justification`                 |`String`                      | レビュー担当者の業務上の理由 (指定されている場合)。                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| レビューの完了時に、結果が手動で適用された場合、決定を適用したユーザーのユーザー id。                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | レビューの決定が適用された日時。                                                          |
| `applyResult`                   |`String`                      | 決定を適用した結果、、、 `NotApplied` `NotFound`また`Success`は`Failed` `NotSupported`のいずれか。                      |
| `accessRecommendation`          |`String`                      | レビュー担当者、 `Approve` `Deny`またはまたは`NotAvailable`のいずれかに表示される、機能で生成された推奨事項。 |


さらに、決定されたアクセスを所有しているオブジェクトのオブジェクトの種類に応じて、追加のプロパティが存在する場合があります。  たとえば、アクセスレビューの決定が特定のユーザーのグループメンバーシップまたはアプリケーションアクセスである場合、アクセスを削除する可能性があるユーザーが次のプロパティを使用して識別されます。

| プロパティ                        | 型                         | 説明                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | アクセスがレビューされたユーザーの id。                                                                                    |
| `userDisplayName`                            |`String`                      | アクセスがレビューされたユーザーの表示名。                                                                                     |
| `userPrincipalName`                            |`String`                      | アクセスがレビューされたユーザーのユーザープリンシパル名。                                                                                     |



## <a name="relationships"></a>リレーションシップ

なし。  この型のオブジェクトは、 [accessreview](accessreview.md)オブジェクトの[決定事項](../api/accessreview-listdecisions.md)と[mydecisions](../api/accessreview-listmydecisions.md)関係を使用して、アクセスレビューから取得できます。

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview に関する決定事項を一覧表示する](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)コレクション| AccessReview の決定事項を取得します。|
|[自分の accessReview の決定事項を一覧表示する](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)コレクション| レビュー担当者として、accessReview の決定事項を取得します。|

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

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
