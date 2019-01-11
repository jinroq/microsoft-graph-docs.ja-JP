---
title: attributeDefinition リソースの種類
description: オブジェクトの属性について説明します。
localization_priority: Normal
ms.openlocfilehash: 63b7f67808ab6695b30f5464d72aed2814e46c5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829681"
---
# <a name="attributedefinition-resource-type"></a>attributeDefinition リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

オブジェクトの属性について説明します。

## <a name="properties"></a>プロパティ

| プロパティ      | 種類      | 説明    |
|:--------------|:----------|:---------------|
|アンカー         |ブール型    | `true`属性は、オブジェクトのアンカーとして使用する必要があります。 場合、 アンカー属性は、オブジェクトを識別する一意の値を持つ必要があり、不変である必要があります。 既定値は `false` です。 のみのいずれか、オブジェクトの属性は、同期をサポートするためにアンカーとして指定する必要があります。 |
|caseExact      |ブール型    |`true`この属性の値を扱う場合、大文字小文字を区別します。 この設定は、同期エンジンが、属性の変更を検出する方法に影響します。|
|metadata       |[metadataEntry](../resources/synchronization-metadataentry.md)    |プロパティをさらに拡張します。 明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。|
|複数値を持つ    |ブール型    |`true`属性は、複数の値を持つことができます。 場合、 既定値は `false` です。|
|可変性     |String     |属性の変更。 使用可能な値: `ReadWrite`、 `ReadOnly`、 `Immutable`、 `WriteOnly`。 既定値は `ReadWrite` です。|
|名前           |String     |属性の名前です。 オブジェクト定義内で一意である必要があります。 null 許容ではありません。|
|必須       |ブール型    |`true`属性が必要な場合です。 必要な属性のいずれかが表示されない場合は、オブジェクトを作成できません。 場合は、同期時に必要な属性値を持たない、既定値が適用されます。 既定値が設定されていない場合、同期はエラーを記録します。|
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
<!-- {
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
