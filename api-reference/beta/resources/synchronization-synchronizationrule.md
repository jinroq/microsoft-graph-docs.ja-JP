---
title: synchronizationRule リソースの種類
description: 同期する対象のオブジェクトを含む、同期エンジンと、方向の同期の実行方法を定義するソース ディレクトリからオブジェクトをコピー先のディレクトリ内のオブジェクトと一致する方法、および属性先のディレクトリにソースから同期されている場合は変換する必要があります。
localization_priority: Normal
ms.openlocfilehash: a739db59a68ece026f9f13dfd22bafce8112f6b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856155"
---
# <a name="synchronizationrule-resource-type"></a>synchronizationRule リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

同期する対象のオブジェクトを含む、同期エンジンと、方向の同期の実行方法を定義するソース ディレクトリからオブジェクトをコピー先のディレクトリ内のオブジェクトと一致する方法、および属性先のディレクトリにソースから同期されている場合は変換する必要があります。

>**注:** 同期規則では、目的のディレクトリにソース ディレクトリからの一方向の同期を定義します。 ソースとターゲットのディレクトリは、ルールのプロパティの一部として定義されます。

同期ルールは、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。

## <a name="properties"></a>プロパティ

| プロパティ      | 種類      | 説明    |
|:--------------|:----------|:---------------|
|編集可能です       |ブール型    |`true`場合は同期ルールをカスタマイズすることができます。`false`場合は、これは読み取り専用で、変更してはなりません。|
|id             |String     |同期規則の識別子です。 同期エンジンによって認識される識別子の 1 つである必要があります。 ルールの識別子を参照して、API によって返される同期テンプレートをサポートします。|
|metadata       |[stringKeyStringValuePair](synchronization-stringkeystringvaluepair.md)コレクション |プロパティをさらに拡張します。 サポート チームによって明示的に指示しない限り、メタデータの値を変更できませんする必要があります。|
|名前           |String     |同期規則の名前を人間が判読できます。 null 許容ではありません。|
|objectMappings |[objectMapping](synchronization-objectmapping.md)コレクション    |ルールでサポートされているオブジェクトのマッピングのコレクションです。 どのオブジェクトを同期する必要があります同期エンジンに指示します。|
|priority       |整数    |[SynchronizationSchema](synchronization-synchronizationschema.md)でその他の規則を基準に優先順位です。 優先度番号が最も小さいルールが最初に処理されます。|
|sourceDirectoryName       |String    |ソース ディレクトリの名前です。 [SynchronizationSchema](synchronization-synchronizationschema.md)でディレクトリの定義のいずれかに一致する必要があります。|
|targetDirectoryName       |String    |コピー先のディレクトリの名前です。 [SynchronizationSchema](synchronization-synchronizationschema.md)でディレクトリの定義のいずれかに一致する必要があります。|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
