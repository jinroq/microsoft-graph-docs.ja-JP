---
title: useridentity の種類
description: 'azure ad のアクセスレビューの場合、この種類は、アクセスレビューのレビュー担当者のための azure ad ユーザー id を表します。  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab8076c5ff24e20006b5a5569dacf4c45d987512
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453979"
---
# <a name="useridentity-type"></a>useridentity の種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

azure ad の[アクセス](accessreviews-root.md)レビューの場合、この種類は、アクセスレビューのレビュー担当者のための azure ad ユーザー id を表します。  
Azure AD 監査ログのコンテキストでは、これは監査アクティビティの開始または影響を受けたユーザー情報を表します。

この型は、 [identity](identity.md)から継承し、ユーザーのユーザープリンシパル名である1つの追加のプロパティを持ちます。

## <a name="methods"></a>メソッド

なし。  [accessreview を作成](../api/accessreview-create.md)するときに、要求の本文にこの種類のオブジェクトを含めることができます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `displayName` | `String` | id の表示名。 これは、常に有効であったり、最新ではない場合があることに注意してください。    |
| `id`          | `String` | ID の一意識別子。  |
| `ipAddress`| `String`| ユーザーがアクティビティを実行するときに使用するクライアント IP アドレスを示します (監査ログのみ)。|
| `userPrincipalName`|`String` | ユーザーの userPrincipalName 属性。 |

## <a name="remarks"></a>注釈

状況によっては、アクターの一意識別子は利用できないことがあります。その場合、ID の **displayName** プロパティが返されますが、**id** プロパティはリソースから失われます。

## <a name="relationships"></a>リレーションシップ

なし。

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[アクセスレビューのレビュー担当者を取得する](../api/accessreview-listreviewers.md) |       [useridentity](useridentity.md)コレクション| accessreview のレビュー担当者を取得します。 |
|[accessreview レビュー担当者を追加する](../api/accessreview-addreviewer.md) |      なし。   |   閲覧者を accessreview に追加します。 |
|[accessreview レビュー担当者を削除する](../api/accessreview-removereviewer.md) | なし。  |   accessreview からレビュー担当者を削除します。 |

## <a name="json-representation"></a>JSON 表記

この型の JSON 表記を次に示します。

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
