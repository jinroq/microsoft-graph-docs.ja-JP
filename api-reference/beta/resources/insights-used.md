---
title: リソースの種類を使用
description: 特定のユーザーによって使用されるドキュメントを表すの把握。 詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: cb41fcb7cef5c9e39f9100ebd1d8c2640f06e2d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885534"
---
# <a name="used-resource-type"></a>リソースの種類を使用

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

特定のユーザーによって使用されるドキュメントを表すの把握。 詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。 内のドキュメントが含まれます。

- OneDrive for Business
- SharePoint

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[リストの使用](../api/insights-list-used.md) |[insights_used](insights-used.md)コレクション| 使用したファイルの一覧を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ              | 種類                      | 説明  |
| -------------         |---------------            | -------------|
| ID                    | String                    | リレーションシップの一意の識別子です。 読み取り専用です。        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | アイテムが最後表示し、ユーザーによって変更された場合について説明します。 読み取り専用です。     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | プロパティは、時にドキュメントをビジュアル化を使用することができます。 読み取り専用です。      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Url およびドキュメントの種類など、使用されているドキュメントのプロパティを参照。 読み取り専用です。     |

## <a name="relationships"></a>リレーションシップ

| プロパティ      | 種類          | 説明  |
| ------------- |---------------| -------------|
| リソース      | Entity        | 使用された項目に移動するために使用します。 ファイルの添付ファイルの種類は、 *fileAttachment*です。 リンクされた添付ファイルの場合は、型は、 *driveItem*です。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
