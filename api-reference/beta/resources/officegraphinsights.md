---
title: officeGraphInsights リソースの種類
description: インサイトとは、高度な分析と機械学習の機能を使って計算されるリレーションシップのことです。 たとえば、ユーザーの周囲で人気急上昇中の OneDrive ドキュメントを特定することができます。
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 8a07cd10622886ad6e367d5311e750454e7bf90b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348876"
---
# <a name="officegraphinsights-resource-type"></a>officeGraphInsights リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

インサイトとは、高度な分析と機械学習の機能を使って計算されるリレーションシップのことです。 たとえば、ユーザーの周囲で人気急上昇中の OneDrive ドキュメントを特定することができます。

インサイトは、次の API によって返されます。

- [Trending](insights-trending.md) - ユーザーの周囲で人気上昇中の OneDrive ドキュメントや SharePoint サイトを返します。
- [Used](insights-used.md) - ユーザーが表示および変更したドキュメントを返します。 ユーザーが OneDrive for Business、SharePoint で使ったドキュメント、メールの添付ファイルとして、あるいは Box、DropBox、Google ドライブなどのソースからのリンクの添付ファイルとして開いたドキュメントが含まれます。
- [Shared](insights-shared.md) - ユーザーと共有されているドキュメントを返します。 ドキュメントは、メールの添付ファイルとして、またはメールで送信した OneDrive for Business のリンクとして共有できます。

各インサイトは、`resourceVisualization` と `resourceReference` の複合値型 (CVT) で返されます。 resourceVisualization CVT には `title` と `previewImageUrl` などのプロパティが含まれます。 Microsoft では、視覚化プロパティを使って Office Delve のようなエクスペリエンスでファイルをレンダリングします。

## <a name="relationships"></a>リレーションシップ

| リレーションシップ      | 型          | 説明  |
| ------------- |---------------| -------------|
| trending      | [trending](insights-trending.md) コレクション       | 計算されたリレーションシップによって人気上昇中のドキュメントを識別します。 人気上昇中のドキュメントは、OneDrive または SharePoint のサイトに保存することができます。   |
| used      | [usedInsight](insights-used.md) コレクション        | 計算されたリレーションシップによってユーザーが表示したり変更したりしたドキュメントを識別します。 ユーザーが OneDrive for Business、SharePoint で使ったドキュメント、メールの添付ファイルとして、あるいは Box、DropBox、Google ドライブなどのソースからのリンクの添付ファイルとして開いたドキュメントが含まれます。  |
| 共有        | [sharedInsight](insights-shared.md) コレクション        | 計算されたリレーションシップによってユーザーが共有しているドキュメントを識別します。 ドキュメントは、メールの添付ファイルとして、またはメールで送信した OneDrive for Business のリンクとして共有できます。   |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.entity",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
