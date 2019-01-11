---
title: extensionSchemaProperty リソースの種類
description: '**extensionSchemaProperty** リソースを使用して、schemaExtension 定義の一部としてプロパティの名前とその種類を定義します。'
localization_priority: Normal
ms.openlocfilehash: 384f60c323ca6c6fb23d2f4811a6d2cb918bf844
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880571"
---
# <a name="extensionschemaproperty-resource-type"></a>extensionSchemaProperty リソースの種類

**extensionSchemaProperty** リソースを使用して、[schemaExtension](schemaextension.md) 定義の一部としてプロパティの名前とその種類を定義します。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|名前|String| スキーマの拡張機能の一部として定義されている厳密に型指定されたプロパティの名前。|
|type|String| スキーマの拡張機能の一部として定義されているプロパティの種類。使用可能な値は、*Binary、Boolean、DateTime、Integer**String* です。詳細については、次の表を参照してください。|

#### <a name="supported-property-data-types"></a>サポート対象のプロパティ データ型 
スキーマ拡張機能でプロパティを定義する場合、次のデータ型がサポートされています。

| プロパティの種類 | 注釈 |
|-------------|------------|
| Binary | 最大 256 バイトです。 |
| Boolean | 連絡先、メッセージ、イベント、投稿ではサポートされていません。 |
| DateTime | ISO 8601 形式で指定する必要があります。UTC で格納されます。 |
| Integer | 32 ビット値です。 連絡先、メッセージ、イベント、投稿ではサポートされていません。 |
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
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
