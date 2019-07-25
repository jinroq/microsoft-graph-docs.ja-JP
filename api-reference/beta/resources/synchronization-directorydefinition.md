---
title: directoryDefinition リソースの種類
description: ディレクトリとそのオブジェクトに関する同期エンジン情報を提供します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56c1f5a6a15f7ab6724feff68aa38eba1ef22694
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888140"
---
# <a name="directorydefinition-resource-type"></a>directoryDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリとそのオブジェクトに関する同期エンジン情報を提供します。 このリソースは、同期エンジンに対して、たとえば、ディレクトリには、**ユーザー**と**グループ**という名前のオブジェクト、これらのオブジェクトに対してサポートされている属性、およびそれらの属性の種類を示します。 オブジェクトと属性を[同期ルール](synchronization-synchronizationrule.md)および[オブジェクトマッピング](synchronization-objectmapping.md)に参加させるには、それらをディレクトリ定義の一部として定義する必要があります。

通常、[同期テンプレート](synchronization-synchronizationtemplate.md)の一部として提供される既定の[同期スキーマ](synchronization-synchronizationschema.md)は、そのディレクトリに最もよく使用されるオブジェクトと属性を定義します。 ただし、ディレクトリでカスタム属性の追加がサポートされている場合は、独自のカスタムオブジェクトまたは属性を使用して、既定の定義を拡張することもできます。 詳細については、「[カスタム属性を使用して同期を構成する](synchronization-configure-with-custom-target-attributes.md)」および「 [configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md)」を参照してください。

ディレクトリ定義は、[同期スキーマ](synchronization-synchronizationschema.md)の一部として更新されます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Discover directoryDefinition](../api/directorydefinition-discover.md) | [directoryDefinition](synchronization-directorydefinition.md) |ディレクトリのスキーマとサポートされているプロパティを検出します。|

## <a name="properties"></a>プロパティ

| プロパティ      | 型      | 説明    |
|:--------------|:----------|:---------------|
|id           |文字列     |ディレクトリ識別子。 null 許容ではありません。|
|metadata       |metadataEntry コレクション    |追加の拡張機能のプロパティ。 明示的に記述されていない限り、メタデータ値は変更しないでください。|
|name           |String     |ディレクトリの名前。 [同期スキーマ](synchronization-synchronizationschema.md)内で一意である必要があります。 null 許容ではありません。|
|対象        |[Objectdefinition](synchronization-objectdefinition.md)コレクション    |ディレクトリでサポートされているオブジェクトのコレクションです。|
|version|String|検出されたバージョンを示す値を取得します。 検出がまだ行われていない場合は、Null。|
|discoveryDateTime|DateTimeOffset| は、ISO 8601 形式を使用した検出日時を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|discoverabilities|string| アプリでサポートされている検出の種類を示す値の読み取り専用です。 使用可能な値: `AttributeDataTypes`、`AttributeNames`、`AttributeReadOnly`、`None`、`ReferenceAttributes`、`UnknownFutureValue`。| 

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "discoverabilities": "String",
  "discoveryDateTime": "DateTimeOffset",
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
