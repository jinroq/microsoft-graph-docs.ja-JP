---
title: コネクタグループリソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543393"
---
# <a name="connectorgroup-resource-type"></a>コネクタグループリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[コネクタグループの取得](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |コネクタのグループオブジェクトのプロパティと関係を読み取ります。|
|[アプリケーションを作成する](../api/connectorgroup-post-applications.md) |[アプリケーション](application.md)| アプリケーションコレクションへの投稿によって、アプリケーションをコネクタグループに関連付けます。|
|[アプリケーションを一覧表示する](../api/connectorgroup-list-applications.md) |[アプリケーション](application.md)コレクション| 関連付けられているアプリケーションオブジェクトのコレクションを取得します。|
|[コネクタを作成する](../api/connectorgroup-post-members.md) |[コネクター](connector.md)| members コレクションへの投稿によってコネクタをコネクタグループに追加します。|
|[メンバーを一覧表示する](../api/connectorgroup-list-members.md) |[connector](connector.md)コレクション| コネクタオブジェクトのコレクションを取得します。|
|[更新](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |コネクタグループオブジェクトを更新します。 |
|[削除](../api/connectorgroup-delete.md) | なし |コネクタグループオブジェクトを削除します。 conector グループを削除する前に、すべてのコネクタを削除する必要があります。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|connectorGroupType|string| グループで使用されるコネクタの種類。 可能な値は`applicationProxy`次のとおりです。|
|id|String| コネクタグループのオブジェクト id|
|isDefault|ブール型 (Boolean)| コネクタグループが既定のコネクタグループであるかどうかを示します。 既定のコネクタグループにすることができ、システムによって設定されるのは、1つのコネクタグループのみです。|
|name|String| コネクタグループに関連付けられている名前。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|アプリケーション|[アプリケーション](application.md)コレクション| 読み取り専用。 Null 許容型。|
|members|[connector](connector.md)コレクション| 読み取り専用。Null 許容型です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectorGroup"
}-->

```json
{
  "connectorGroupType": "string",
  "id": "String (identifier)",
  "isDefault": true,
  "name": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connectorGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/connectorgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
