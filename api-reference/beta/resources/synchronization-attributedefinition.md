---
title: attributeDefinition リソースの種類
description: オブジェクトの属性について説明します。
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643917"
---
# <a name="attributedefinition-resource-type"></a>attributeDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オブジェクトの属性について説明します。

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|アンカー         |Boolean    | `true`属性は、オブジェクトのアンカーとして使用する必要があります。 場合、 アンカー属性は、オブジェクトを識別する一意の値を持つ必要があり、不変である必要があります。 既定値は `false` です。 のみのいずれか、オブジェクトの属性は、同期をサポートするためにアンカーとして指定する必要があります。 |
|caseExact      |Boolean    |`true`この属性の値を扱う場合、大文字小文字を区別します。 この設定は、同期エンジンが、属性の変更を検出する方法に影響します。|
|metadata       |[metadataEntry](../resources/synchronization-metadataentry.md)    |プロパティをさらに拡張します。 明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。|
|複数値を持つ    |Boolean    |`true`属性は、複数の値を持つことができます。 場合、 既定値は `false` です。|
|可変性     |String     |属性の変更。 使用可能な値: `ReadWrite`、 `ReadOnly`、 `Immutable`、 `WriteOnly`。 既定値は `ReadWrite` です。|
|name           |String     |属性の名前です。 オブジェクト定義内で一意である必要があります。 null 許容型ではありません。|
|必須       |Boolean    |`true`属性が必要な場合です。 必要な属性のいずれかが表示されない場合は、オブジェクトを作成できません。 場合は、同期時に必要な属性値を持たない、既定値が適用されます。 既定値が設定されていない場合、同期はエラーを記録します。|
|referencedObjects|[referencedObject](../resources/synchronization-referencedobject.md) |属性の場合`reference`参照されるオブジェクトのリストを入力します。 (たとえば、、`manager`属性のリストが`User`として参照されているオブジェクト)。|
|type           |String     |属性の値の種類。 使用可能な値は、`String`、`Integer`、`Reference`、`Binary`、`Boolean` です。 既定値は `String` です。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
