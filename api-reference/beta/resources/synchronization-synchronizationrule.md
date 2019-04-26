---
title: 同期規則リソースの種類
description: 同期エンジンに対して同期を実行する方法を定義します。どのオブジェクトを同期するか、どの方向に、どのようにソースディレクトリのオブジェクトをターゲットディレクトリのオブジェクトと照合するか、どのように属性を使用するかを指定します。ソースとターゲットディレクトリの同期時に変換する必要があります。
localization_priority: Normal
ms.openlocfilehash: b881c73d8fec8dc6b342192195d486807c744cf7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340027"
---
# <a name="synchronizationrule-resource-type"></a>同期規則リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同期エンジンに対して同期を実行する方法を定義します。どのオブジェクトを同期するか、どの方向に、どのようにソースディレクトリのオブジェクトをターゲットディレクトリのオブジェクトと照合するか、どのように属性を使用するかを指定します。ソースとターゲットディレクトリの同期時に変換する必要があります。

>**注:** 同期ルールは、ソースディレクトリからターゲットディレクトリへの一方向での同期を定義します。 ソースディレクトリとターゲットディレクトリは、ルールのプロパティの一部として定義されます。

同期ルールは、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|可能       |Boolean    |`true`同期ルールをカスタマイズできる場合は、`false`このルールは読み取り専用であり、変更する必要はありません。|
|id             |String     |同期ルール識別子。 同期エンジンで認識される識別子のいずれかである必要があります。 サポートされているルール識別子は、API によって返される同期テンプレートにあります。|
|metadata       |[stringkeystringvaluepair](synchronization-stringkeystringvaluepair.md)コレクション |追加の拡張機能のプロパティ。 サポートチームによって明示的に指示されていない限り、メタデータ値は変更しないでください。|
|name           |String     |ユーザーが読み取ることができる同期ルールの名前。 null 許容型ではありません。|
|objectmappings |[objectmapping](synchronization-objectmapping.md)コレクション    |ルールでサポートされているオブジェクトマッピングのコレクション。 同期するオブジェクトを同期エンジンに通知します。|
|priority       |整数    |[同期スキーマ](synchronization-synchronizationschema.md)内の他のルールに対する優先度。 優先度が最も低いルールが最初に処理されます。|
|sourceDirectoryName       |String    |ソースディレクトリの名前。 は、[同期スキーマ](synchronization-synchronizationschema.md)のディレクトリ定義のいずれかと一致している必要があります。|
|targetDirectoryName       |String    |ターゲットディレクトリの名前。 は、[同期スキーマ](synchronization-synchronizationschema.md)のディレクトリ定義のいずれかと一致している必要があります。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
