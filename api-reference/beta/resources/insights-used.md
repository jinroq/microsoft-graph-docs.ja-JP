---
title: リソースの種類を使用
description: 特定のユーザーによって使用されるドキュメントを表すの把握。 詳細情報は、ユーザーが表示またはアクセスする最も適切なドキュメントを返します。 内のドキュメントが含まれます。
ms.openlocfilehash: 3c82d268a67ef52d0ddfdad9193558080048ad6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072327"
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

| プロパティ              | 型                      | 説明  |
| -------------         |---------------            | -------------|
| id                    | String                    | リレーションシップの一意の識別子です。 読み取り専用です。        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | アイテムが最後表示し、ユーザーによって変更された場合について説明します。 読み取り専用です。     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | プロパティは、時にドキュメントをビジュアル化を使用することができます。 読み取り専用      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Url およびドキュメントの種類など、使用されているドキュメントのプロパティを参照。 読み取り専用     |

## <a name="relationships"></a>リレーションシップ

| プロパティ      | 型          | 説明  |
| ------------- |---------------| -------------|
| リソース      | エンティティ        | 使用された項目に移動するために使用します。 ファイルの添付ファイルの種類は、 *fileAttachment*です。 リンクされた添付ファイルの場合は、型は、 *driveItem*です。 |

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