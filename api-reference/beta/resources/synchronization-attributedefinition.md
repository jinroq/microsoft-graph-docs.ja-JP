---
title: attributeDefinition リソースの種類
description: オブジェクトの属性を表します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3652a6d09d363a4f14227752506ba5d670dfd6fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008006"
---
# <a name="attributedefinition-resource-type"></a>attributeDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オブジェクトの属性を表します。

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|位置         |Boolean    | `true`オブジェクトのアンカーとして属性を使用する必要があるかどうか。 アンカー属性には、オブジェクトを識別する一意の値を指定する必要があります。不変にする必要があります。 既定値は `false` です。 同期をサポートするには、オブジェクトの属性の1つだけをアンカーとして指定する必要があります。 |
|ケース Exact      |Boolean    |`true`この属性の値を大文字と小文字を区別して扱う必要がある場合。 この設定は、同期エンジンが属性の変更を検出する方法に影響します。|
|metadata       |[Metadataentry](../resources/synchronization-metadataentry.md)コレクション   |追加の拡張機能のプロパティ。 明示的に記述されていない限り、メタデータ値は変更しないでください。|
|複数値    |Boolean    |`true`属性に複数の値を設定できる場合。 既定値は `false` です。|
|mutability     |String     |属性の変わり可能性。 可能な値は`ReadWrite`、 `ReadOnly`、 `Immutable`、 `WriteOnly`、です。 既定値は `ReadWrite` です。|
|name           |String     |属性の名前。 オブジェクト定義内で一意である必要があります。 null 許容ではありません。|
|必須       |Boolean    |`true`属性が必要かどうか。 必要な属性のいずれかが不足している場合は、オブジェクトを作成できません。 同期時に必須属性に値がない場合は、既定値が使用されます。 既定値が設定されていない場合は、同期によってエラーが記録されます。|
|referencedopivot|[Referencedobject](../resources/synchronization-referencedobject.md)コレクション |Type の属性の場合は、参照されているオブジェクト`manager`を一覧表示`User`します (たとえば、属性が参照されるオブジェクトとしてリストになります)。 `reference`|
|type           |String     |属性値の型。 使用可能な値は、`String`、`Integer`、`Reference`、`Binary`、`Boolean` です。 既定値は `String` です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
