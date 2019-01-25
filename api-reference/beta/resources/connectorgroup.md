---
title: connectorGroup リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: de405d2f0cbe0417271ab54e66c5c30073d8ee7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517499"
---
# <a name="connectorgroup-resource-type"></a>connectorGroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ConnectorGroup を取得します。](../api/connectorgroup-get.md) | [connectorGroup](connectorgroup.md) |ConnectorGroup オブジェクトのプロパティと関係を参照してください。|
|[アプリケーションを作成します。](../api/connectorgroup-post-applications.md) |[application](application.md)| コネクタ グループにアプリケーションを関連付けるアプリケーションのコレクションへの投稿。|
|[アプリケーション一覧](../api/connectorgroup-list-applications.md) |[アプリケーション](application.md)コレクション| 関連付けられているアプリケーション オブジェクトのコレクションを取得します。|
|[コネクタを作成します。](../api/connectorgroup-post-members.md) |[Connector](connector.md)| 図形をグループ化するメンバーのコレクションへの投稿、コネクタを追加します。|
|[メンバーを一覧表示する](../api/connectorgroup-list-members.md) |[コネクタ](connector.md)のコレクション| コネクタ オブジェクトのコレクションを取得します。|
|[Update](../api/connectorgroup-update.md) | [connectorGroup](connectorgroup.md)    |ConnectorGroup オブジェクトを更新します。 |
|[Delete](../api/connectorgroup-delete.md) | なし |ConnectorGroup オブジェクトを削除します。 すべてのコネクタは、コネクタのグループを削除する前に削除をする必要があります。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|connectorGroupType|string| グループで使用するコネクタの種類です。 使用可能な値: `applicationProxy`。|
|id|String| ConnectorGroup のオブジェクト id|
|isDefault|ブール値| ConnectorGroup がコネクタの既定のグループであるかどうかを示します。 のみ、1 つのコネクタ グループはデフォルトの connectorGroup をすることができ、システムによって設定されます。|
|name|String| ConnectorGroup に関連付けられている名前です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|アプリケーション|[アプリケーション](application.md)コレクション| 読み取り専用。Null 許容型。|
|members|[コネクタ](connector.md)のコレクション| 読み取り専用です。Null 許容型。|

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
