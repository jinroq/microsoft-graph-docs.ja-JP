---
title: synchronizationTemplate リソースの種類
description: " すべてのユーザーは、同期スキーマを含む、既定の設定を表示するテンプレートを取得できます。"
ms.openlocfilehash: 90850ad43fdd14fc38ff6ae8cfa97f47806a289d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070566"
---
# <a name="synchronizationtemplate-resource-type"></a>synchronizationTemplate リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特定のアプリケーションの構成済みの同期設定を提供します。 これらの設定は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)の既定で使用されます。 アプリケーション開発者は、テンプレートを指定します。すべてのユーザーは、[同期スキーマ](synchronization-synchronizationschema.md)を含む、既定の設定を表示するテンプレートを取得できます。

アプリケーションは、複数のテンプレートを提供し、既定のテンプレートを指定できます。 関心のアプリケーションの複数のテンプレートがある場合は、お客様のニーズに最も適したどちらかを決定するアプリケーション固有のガイダンスをシークします。

## <a name="methods"></a>メソッド

| メソッド        | 戻り値の型               | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[synchronizationTemplate](synchronization-synchronizationtemplate.md)コレクション  |アプリケーションまたはアプリケーションのインスタンス (サービス主体) の使用可能なテンプレートの一覧を表示します。|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |プロパティと**synchronizationTemplate**オブジェクトの関係を参照してください。|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>プロパティ

| プロパティ      | 型                      | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |String                     |テンプレートの一意の識別子です。|
|applicationId  |文字列型 (String)                     |このテンプレートが属するアプリケーションの識別子です。|
|既定値です。        |ブール値                    |`true`場合は、アプリケーションの既定の設定をするのには、このテンプレートをお勧めします。|
|説明    |文字列                     |テンプレートの説明です。|
|検出可能   |String                     |`true`このテンプレートは、アプリケーションのインスタンス (サービス主体) の使用可能なテンプレートのコレクションに表示されます。 場合、|
|factoryTag     |String                     |同期エンジンでサポートされている既知の工場出荷時のタグの 1 つです。 **FactoryTag**は、このテンプレートに基づいてジョブを処理するときに使用する実装を同期エンジンを指示します。|
|metadata       |metadataEntry コレクション   |プロパティをさらに拡張します。 明示的に記載されている、しない限り、メタデータの値を変更できませんする必要があります。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ      | 型      |説明|
|:------------------|:----------|:----------|
|スキーマ             |[synchronizationSchema](synchronization-synchronizationschema.md)     |このテンプレートに基づいて、ジョブの既定の同期スキーマです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->