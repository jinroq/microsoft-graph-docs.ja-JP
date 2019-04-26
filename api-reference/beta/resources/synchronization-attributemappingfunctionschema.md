---
title: attributeMappingFunctionSchema リソースの種類
description: 同期時に値を変換するために属性マッピングで使用できる関数について説明します。
localization_priority: Normal
ms.openlocfilehash: e2c0139f7c797c3f519cc638561b09f611018b28
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582094"
---
# <a name="attributemappingfunctionschema-resource-type"></a>attributeMappingFunctionSchema リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同期時に値を変換するために[属性マッピング](synchronization-attributemapping.md)で使用できる関数について説明します。

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[List](../api/synchronization-synchronizationschema-functions.md) | [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション|サポートされている属性マッピング関数を一覧表示します。|

## <a name="properties"></a>プロパティ

| プロパティ                   | 型                      | 説明    |
|:---------------------------|:-------------------------|:---------------|
|name                        |String                    |オペレーター名。 |
|parameters                  |[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)コレクション  |関数パラメータのコレクション。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
