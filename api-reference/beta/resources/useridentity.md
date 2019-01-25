---
title: 型を割り当てられていません
description: 'Azure AD のレビューにアクセスして、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab8076c5ff24e20006b5a5569dacf4c45d987512
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529468"
---
# <a name="useridentity-type"></a>型を割り当てられていません

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD[アクセスの確認](accessreviews-root.md)をするは、この型は、アクセス レビューのレビュー担当者の Azure AD ユーザー id を表します。  
Azure AD の監査ログのコンテキストでは、開始、または監査活動の影響を受けたユーザーの情報を表します。

このタイプは、[アイデンティティ](identity.md)を継承し、追加の 1 つのプロパティ、ユーザーのユーザー プリンシパル名を持ちます。

## <a name="methods"></a>メソッド

なし  要求の本文にこの型のオブジェクトを含めますと[、accessReview を作成](../api/accessreview-create.md)します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `displayName` | `String` | Id の表示名です。 このできない可能性がある利用可能なまたは最新の状態に注意してください。    |
| `id`          | `String` | ID の一意識別子。  |
| `ipAddress`| `String`| アクティビティ (監査ログのみ) を実行するユーザーによって使用されるクライアントの IP アドレスを示します。|
| `userPrincipalName`|`String` | ユーザーの userPrincipalName 属性です。 |

## <a name="remarks"></a>注釈

状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview のレビュー担当者を取得します。](../api/accessreview-listreviewers.md) |       コレクションを[割り当てられていません](useridentity.md)| AccessReview のレビュー担当者を取得します。 |
|[AccessReview の校閲者を追加します。](../api/accessreview-addreviewer.md) |      なし。   |   AccessReview には、レビュー担当者を追加します。 |
|[AccessReview のレビュー担当者を削除します。](../api/accessreview-removereviewer.md) | なし。  |   AccessReview からレビュー担当者を削除します。 |

## <a name="json-representation"></a>JSON 表記

ここでは、型の JSON 表現です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
 "userPrincipalName": "String"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
