---
title: synchronizationSchema リソースの種類
description: オブジェクトがどのようになるかを定義する同期し、同期する方法です。 同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。 通常にするいくつかの属性のマッピングをカスタマイズするかを特定の条件を満たすオブジェクトのみを同期するスコープのフィルターを追加します。
localization_priority: Normal
ms.openlocfilehash: e7bb91ef473a04552c4c5f33ffc9d54eb86a9b7a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515931"
---
# <a name="synchronizationschema-resource-type"></a>synchronizationSchema リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

オブジェクトがどのようになるかを定義する同期し、同期する方法です。 同期スキーマには、特定の同期ジョブのセットアップ情報のほとんどが含まれています。 通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズまたはを特定の条件を満たすオブジェクトのみを同期する[スコープのフィルター](synchronization-filter.md)が追加されます。

次のセクションでは、同期スキーマの高度なコンポーネントについて説明します。

## <a name="directory-definitions"></a>ディレクトリの定義

[ディレクトリの定義](synchronization-directorydefinition.md)では、ディレクトリとそのオブジェクトの同期エンジンに関する情報を提供します。 などのディレクトリの定義では、同期エンジンが指示、Azure AD ディレクトリが**ユーザー**と**グループ**、それらのオブジェクトとそれらの属性の型の属性はサポートされてをという名前のオブジェクトを持っています。 同期規則とオブジェクトのマッピングで使用する特定のオブジェクトと属性の順序でディレクトリの定義の一部として定義する必要があります。

## <a name="synchronization-rules"></a>同期ルール

[同期ルール](synchronization-synchronizationrule.md)は、同期の設定の中核です。 同期を実行する方法、同期エンジンを定義する、どのようなオブジェクトを含む同期するか、ソース ディレクトリからオブジェクトのコピー先のディレクトリ内のオブジェクトとの照合方法と、属性がどのようにする必要がありますか目的のディレクトリにソースから同期されている場合に変換されます。 

## <a name="object-mappings"></a>オブジェクトのマッピング

[オブジェクトのマッピング](synchronization-objectmapping.md)は、同期ルールの主な部分です。 どのように特定のオブジェクト同期する必要があるソースからターゲット ・ ディレクトリに各オブジェクトのマッピングを定義します。 マッピングがコピー先のディレクトリ内のオブジェクトのソース ディレクトリ内のオブジェクトの照合方法を定義する具体的には、どのような (ある場合) し、オブジェクトを提供するかどうか、オブジェクトの属性を変換する方法を決定するフィルターのスコープを使用する必要があります同期されているソースからコピー先のディレクトリにします。

## <a name="methods"></a>メソッド

| メソッド        | 戻り値の型               | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|[スキーマを取得します](../api/synchronization-synchronizationschema-get.md)    |[synchronizationSchema](synchronization-synchronizationschema.md)   |**SynchronizationSchema**オブジェクトのプロパティと関係を参照してください。|
|[スキーマを更新します。](../api/synchronization-synchronizationschema-update.md)    |なし   |同期スキーマを更新します。 |
|[スキーマを削除します。](../api/synchronization-synchronizationschema-delete.md)    |なし   |スキーマを既定の構成にリセットする、カスタマイズされたスキーマを削除します。 |
|[リスト フィルターの演算子](../api/synchronization-synchronizationschema-filteroperators.md)    |[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)コレクション   |スコープ フィルターでサポートされているすべての演算子の一覧を表示します。 |
|[リストの属性が関数のマッピング](../api/synchronization-synchronizationschema-functions.md)    |[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション   |属性マッピングの式でサポートされているすべての関数の一覧を表示します。 |
|[属性マッピングの式を解析します。](../api/synchronization-synchronizationschema-parseexpression.md)|[parseExpressionResponse](synchronization-parseexpressionresponse.md)|[AttributeMappingSource に文字列を解析します。|(../resources/synchronization_attributemappingsource.md) オブジェクト。|


## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|directories            |[directoryDefinition](synchronization-directorydefinition.md)コレクション   |ディレクトリおよび[synchronizationJob](synchronization-synchronizationjob.md)または[synchronizationTemplate](synchronization-synchronizationtemplate.md)の一部であるオブジェクトについて説明します。 |
|synchronizationRules   |[synchronizationRule](synchronization-synchronizationrule.md)コレクション   |[SynchronizationJob](synchronization-synchronizationjob.md)または[synchronizationTemplate](synchronization-synchronizationtemplate.md)、用に構成された同期規則のコレクション |
|version                |String                             |スキーマ変更のたびに自動的に更新、スキーマのバージョン。|


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
