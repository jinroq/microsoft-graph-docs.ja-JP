---
title: 共有リソースの種類
description: または特定のユーザーが共有ファイルを表すの把握。 次の共有ファイルがサポートされています。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 289523f836d7b8080f7317e4d11301c71314ba93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880613"
---
# <a name="shared-resource-type"></a>共有リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

または特定のユーザーが共有ファイルを表すの把握。 次の共有ファイルがサポートされています。

- 電子メールや会議に直接接続されているファイルを招待します。
- 名刺と SharePoint 現代の添付ファイル、ビジネスおよびユーザーが、リンクとして電子メールで共有する SharePoint の OneDrive に格納されているファイルの OneDrive です。

**注**: データの共有 API の結果を作成するのに現在進行中です。 リリース後の最初の週で不足しているいくつかのデータがある可能性があります。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[共有リスト](../api/insights-list-shared.md) |[insights_shared](insights-shared.md)コレクション| 共有ファイルの一覧を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ              | 種類                      | 説明  |
| -------------         |---------------            | -------------|
| ID                    | String                    | リレーションシップの一意の識別子です。 読み取り専用です。        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | 共有アイテムに関する詳細情報です。 読み取り専用です。        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | プロパティは、時にドキュメントをビジュアル化を使用することができます。 読み取り専用です。      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Url およびドキュメントの種類など、共有ドキュメントのプロパティを参照します。 読み取り専用です。       |

## <a name="relationships"></a>リレーションシップ

| プロパティ      | 種類          | 説明  |
| ------------- |---------------| -------------|
| リソース      | Entity        | 共有されている項目に移動するために使用します。 ファイルの添付ファイルの種類は、 *fileAttachment*です。 リンクされた添付ファイルの場合は、型は、 *driveItem*です。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
