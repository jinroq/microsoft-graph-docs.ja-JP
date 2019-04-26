---
title: /リソースの種類 (sharepoint)
description: または特定のユーザーによって共有されているファイルを表す洞察。 次の共有ファイルがサポートされています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 128a85bb9aa2e9f51d2393029cce3c27f8c4e6f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339992"
---
# <a name="sharedinsight-resource-type"></a>/リソースの種類 (sharepoint)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

または特定のユーザーによって共有されているファイルを表す洞察。 次の共有ファイルがサポートされています。

- 電子メールまたは会議の招待に直接添付されたファイル。
- onedrive for Bussiness および sharepoint モダン添付ファイル-ユーザーが電子メールのリンクとして共有する、onedrive for business および sharepoint に格納されているファイル。

**注**: 現在、データを使用して共有 API の結果を設定する作業を行っています。 リリース後の最初の週に、一部のデータが欠落している場合があります。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[共有リスト](../api/insights-list-shared.md) |[insights_shared](insights-shared.md)コレクション| 共有ファイルの一覧を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ              | 型                      | 説明  |
| -------------         |---------------            | -------------|
| id                    | String                    | リレーションシップの一意識別子。 読み取り専用です。        |
| lastshared            | [sharingDetail](insights-sharingdetail.md)                | 共有アイテムの詳細。 読み取り専用です。        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | ユーザーの作業でドキュメントをビジュアル化するために使用できるプロパティ。 読み取り専用      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | ドキュメントの url や種類など、共有ドキュメントの参照プロパティ。 読み取り専用       |

## <a name="relationships"></a>リレーションシップ

| プロパティ      | 型          | 説明  |
| ------------- |---------------| -------------|
| リソース      | entity コレクション | 共有されているアイテムに移動するために使用します。 添付ファイルの場合、type は*fileattachment*になります。 リンクされた添付ファイルの場合、種類は [*ドライブ] 項目*です。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です
<!--{
  "blockType":"resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
