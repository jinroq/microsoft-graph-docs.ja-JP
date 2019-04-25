---
title: resourcevisualization リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550738"
---
# <a name="resourcevisualization-resource-type"></a>resourcevisualization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Insights](insights.md)のプロパティを含む複合型。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

```json
{
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 型          | 説明  |
| -------------         |---------------| -------------|
| title                 | String        | アイテムのタイトルテキスト。               |
| type              | String        | アイテムのメディアの種類。 特定の種類に基づいて特定のファイルをフィルター処理するために使用できます。 サポートされる種類については、以下を参照してください。 |
| mediaType             | String        | アイテムのメディアの種類。 は、サポートされている IANA メディア Mime タイプに基づいて、特定の種類のファイルをフィルター処理するために使用できます。 すべてのメディア Mime タイプがサポートされるわけではないことに注意してください。 |
| previewImageUrl       | String        | アイテムのプレビューイメージの先頭になる URL。 |
| previewText           | String        | アイテムのプレビューテキスト。 |
| containerWebUrl       | String        | アイテムが格納されるフォルダーへのパス。 |
| containerDisplayName  | String        | アイテムが格納されている場所を示す文字列。 たとえば、SharePoint サイトの名前、またはアイテムを格納している OneDrive の所有者を識別するユーザー名。  |
| containerType         | String | ファイルが格納されているコンテナーの種類によるフィルター処理に使用できます。 サイト、onedrive business など。       |

## <a name="type-property-values"></a>Type プロパティの値
-   PowerPoint
-   Word
-   Excel
-   文書
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   プロジェクト
-   Access
-   メール
-   .csv
-   アーカイブ
-   Xps
-   オーディオ
-   ビデオ
-   イメージ
-   Web
-   テキスト
-   Xml
-   Story
-   externalcontent
-   フォルダー
-   その他

クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>containerType プロパティの値
サポートされている種類は、[洞察](insights.md)がファイルを返すコンテナーによって異なる場合があります。 たとえば、[共有](insights-shared.md)された洞察のみが、' DropBox '、' Box '、' gdrive ' からファイルを返します。

-   onedrive business
-   サイト
-   メール
-   DropBox
-   検索ボックス
-   gdrive

クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
