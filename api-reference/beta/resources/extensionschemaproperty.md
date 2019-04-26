---
title: extensionSchemaProperty リソースの種類
description: '**extensionSchemaProperty** リソースを使用して、schemaExtension 定義の一部としてプロパティの名前とその種類を定義します。'
localization_priority: Normal
ms.openlocfilehash: 05fb5eb94f760bce26ba09bf3e8e862ff5fd2fb8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340266"
---
# <a name="extensionschemaproperty-resource-type"></a>extensionSchemaProperty リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**extensionSchemaProperty** リソースを使用して、[schemaExtension](schemaextension.md) 定義の一部としてプロパティの名前とその種類を定義します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|name|String| スキーマ拡張機能の一部として定義された厳密に型指定されたプロパティの名前。|
|type|String| スキーマの拡張機能の一部として定義されているプロパティの種類。使用可能な値は、*Binary、Boolean、DateTime、Integer**String* です。詳細については、次の表を参照してください。|

#### <a name="supported-property-data-types"></a>サポート対象のプロパティ データ型 
スキーマ拡張機能でプロパティを定義する場合、次のデータ型がサポートされています。

| プロパティの種類 | 注釈 |
|-------------|------------|
| Binary | 最大 256 バイトです。 |
| Boolean | メッセージ、イベント、投稿ではサポートされていません。 |
| DateTime | ISO 8601 形式で指定する必要があります。UTC で格納されます。 |
| 整数 | 32 ビット値です。メッセージ、イベント、投稿ではサポートされていません。 |
| String | 最大 256 文字です。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
