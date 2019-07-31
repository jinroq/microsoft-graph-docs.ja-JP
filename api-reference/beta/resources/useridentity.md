---
title: userIdentity の種類
description: 'Azure AD のアクセスレビューの場合、この種類は、アクセスレビューのレビュー担当者のための Azure AD ユーザー id を表します。  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 21342efd10f5e6f66db795a781eb3f0e333975a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007453"
---
# <a name="useridentity-type"></a>userIdentity の種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD[アクセスレビュー](accessreviews-root.md)の場合、この種類は、アクセスレビューの作成者またはレビュー担当者のための azure ad ユーザー id を表します。  
Azure AD 監査ログのコンテキストでは、これは監査アクティビティの開始または影響を受けたユーザー情報を表します。

この型は、 [identity](identity.md)から継承し、ユーザーのユーザープリンシパル名である1つの追加のプロパティを持ちます。

## <a name="methods"></a>メソッド

なし。  [AccessReview を作成](../api/accessreview-create.md)するときに、要求の本文にこの種類のオブジェクトを含めることができます。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| `displayName` | `String` | Id の表示名。 これは、常に有効であったり、最新ではない場合があることに注意してください。    |
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
|[アクセスレビューのレビュー担当者を取得する](../api/accessreview-listreviewers.md) |       [Useridentity](useridentity.md)コレクション| AccessReview のレビュー担当者を取得します。 |
|[AccessReview レビュー担当者を追加する](../api/accessreview-addreviewer.md) |      なし。   |   閲覧者を accessReview に追加します。 |
|[AccessReview レビュー担当者を削除する](../api/accessreview-removereviewer.md) | なし。  |   AccessReview からレビュー担当者を削除します。 |

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
  "userPrincipalName": "String",
  "ipAddress": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
