---
title: 同期テンプレートリソースの種類
description: " すべてのユーザーがテンプレートを取得して、同期スキーマを含む既定の設定を確認できます。"
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 125b8fe81aedc285da33380c3043827c7c534ab8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620648"
---
# <a name="synchronizationtemplate-resource-type"></a>同期テンプレートリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定のアプリケーションに事前に構成された同期設定を提供します。 これらの設定は、テンプレートに基づくすべての[同期ジョブ](synchronization-synchronizationjob.md)に対して既定で使用されます。 アプリケーション開発者は、テンプレートを指定します。すべてのユーザーがテンプレートを取得して、[同期スキーマ](synchronization-synchronizationschema.md)を含む既定の設定を確認できます。

アプリケーションに対して複数のテンプレートを提供し、既定のテンプレートを指定することができます。 目的のアプリケーションで複数のテンプレートが使用可能な場合は、アプリケーション固有のガイダンスを検索して、ニーズに最適なものを決定します。

## <a name="methods"></a>メソッド

| メソッド        | 戻り値の型               | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|[List](../api/synchronization-synchronizationtemplate-list.md)    |[同期テンプレート](synchronization-synchronizationtemplate.md)のコレクション  |アプリケーションまたはアプリケーションインスタンス (サービスプリンシパル) に対して使用可能なテンプレートを一覧表示します。|
|[Get](../api/synchronization-synchronizationtemplate-get.md)      |[同期テンプレート](synchronization-synchronizationtemplate.md)   |**同期テンプレート**オブジェクトのプロパティとリレーションシップを読み取ります。|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a>プロパティ

| プロパティ      | 型                      | 説明                  |
|:--------------|:--------------------------|:-----------------------------|
|id             |String                     |一意のテンプレート識別子。|
|applicationId  |String                     |このテンプレートが属しているアプリケーションの識別子。|
|既定値です。        |Boolean                    |`true`このテンプレートをアプリケーションの既定として使用することをお勧めします。|
|description    |String                     |テンプレートの説明。|
|発見   |String                     |`true`このテンプレートをアプリケーションインスタンス (サービスプリンシパル) で使用可能なテンプレートのコレクションに表示する必要がある場合。|
|factoryTag     |String                     |同期エンジンでサポートされている、既知の出荷済みのタグの1つ。 **FactoryTag**は、このテンプレートに基づいてジョブを処理するときに使用する実装を同期エンジンに通知します。|
|metadata       |metadataEntry コレクション   |追加の拡張機能のプロパティ。 明示的に記述されていない限り、メタデータ値は変更しないでください。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ      | 型      |説明|
|:------------------|:----------|:----------|
|スキーマ             |[同期スキーマ](synchronization-synchronizationschema.md)     |このテンプレートに基づくジョブの既定の同期スキーマ。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
