---
title: 同期スキーマリソースの種類
description: 同期されるオブジェクトと、それらの同期方法を定義します。 同期スキーマには、特定の同期ジョブの設定情報の大部分が含まれています。 通常、属性マッピングの一部をカスタマイズするか、特定の条件を満たすオブジェクトのみを同期するスコープフィルターを追加します。
localization_priority: Normal
ms.openlocfilehash: 8fd43a028a7d94b6d4a7c1e5d3c47520bff507ec
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339874"
---
# <a name="synchronizationschema-resource-type"></a>同期スキーマリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

同期されるオブジェクトと、それらの同期方法を定義します。 同期スキーマには、特定の同期ジョブの設定情報の大部分が含まれています。 通常、[属性マッピング](synchronization-attributemapping.md)の一部をカスタマイズするか、特定の条件を満たすオブジェクトのみを同期する[スコープフィルター](synchronization-filter.md)を追加します。

次のセクションでは、同期スキーマの高レベルのコンポーネントについて説明します。

## <a name="directory-definitions"></a>ディレクトリ定義

[ディレクトリ定義](synchronization-directorydefinition.md)は、ディレクトリとそのオブジェクトに関する同期エンジン情報を提供します。 たとえば、ディレクトリ定義は、Azure AD ディレクトリに、**ユーザー**と**グループ**という名前のオブジェクトがあり、それらのオブジェクトに対してサポートされている属性、およびそれらの属性の種類があることを同期エンジンに通知します。 同期ルール/オブジェクトマッピングで特定のオブジェクトおよび属性を使用するためには、それらをディレクトリ定義の一部として定義する必要があります。

## <a name="synchronization-rules"></a>同期ルール

[同期ルール](synchronization-synchronizationrule.md)は、同期のセットアップの中核となります。 同期を実行する方法、同期する必要のあるオブジェクト、ソースディレクトリのオブジェクトとターゲットディレクトリのオブジェクトとの比較、属性の適用方法など、同期エンジンを定義します。ソースからターゲットディレクトリへの同期時に変換されます。 

## <a name="object-mappings"></a>オブジェクトマッピング

[オブジェクトマッピング](synchronization-objectmapping.md)は、同期ルールの主な部分です。 各オブジェクトマッピングは、指定されたオブジェクトをソースからターゲットディレクトリへ同期する方法を定義します。 特に、マッピングでは、ソースディレクトリ内のオブジェクトをターゲットディレクトリのオブジェクトと照合する方法、オブジェクトをプロビジョニングするかどうか、およびオブジェクト属性をどのように変換するかを決定するために使用するスコープフィルターを定義します。ソースからターゲットディレクトリに同期されている場合。

## <a name="methods"></a>メソッド

| メソッド        | 戻り値の型               | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|[スキーマを取得する](../api/synchronization-synchronizationschema-get.md)    |[同期スキーマ](synchronization-synchronizationschema.md)   |**同期スキーマ**オブジェクトのプロパティとリレーションシップを読み取ります。|
|[スキーマを更新する](../api/synchronization-synchronizationschema-update.md)    |なし   |同期スキーマを更新します。 |
|[スキーマの削除](../api/synchronization-synchronizationschema-delete.md)    |なし   |カスタマイズしたスキーマを削除し、スキーマを既定の構成にリセットします。 |
|[リストフィルター演算子](../api/synchronization-synchronizationschema-filteroperators.md)    |[filter演算子スキーマ](../resources/synchronization-filteroperatorschema.md)コレクション   |スコープフィルターでサポートされているすべての演算子を一覧表示します。 |
|[リスト属性マッピング関数](../api/synchronization-synchronizationschema-functions.md)    |[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)コレクション   |属性マッピング式でサポートされているすべての関数を一覧表示します。 |
|[解析属性マッピング式](../api/synchronization-synchronizationschema-parseexpression.md)|[parseexpression response](synchronization-parseexpressionresponse.md)|文字列式を解析し、[attributeMappingSource|(../resources/synchronization_attributemappingsource.md) オブジェクト。|


## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|移動            |[directorydefinition](synchronization-directorydefinition.md)コレクション   |[同期ジョブ](synchronization-synchronizationjob.md)または[同期のテンプレート](synchronization-synchronizationtemplate.md)の一部であるディレクトリとオブジェクトについて説明します。 |
|同期規則   |[同期ルール](synchronization-synchronizationrule.md)のコレクション   |同期ジョブまたは同期[ジョブ](synchronization-synchronizationjob.md)[テンプレート](synchronization-synchronizationtemplate.md)用に構成されている同期ルールのコレクション。 |
|version                |String                             |スキーマのバージョンは、すべてのスキーマ変更によって自動的に更新されます。|


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
  "suppressions": []
}
-->
