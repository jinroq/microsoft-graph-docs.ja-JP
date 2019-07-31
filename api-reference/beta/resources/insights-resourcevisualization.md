---
title: resourceVisualization リソースの種類
description: Insights のプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ce18edcdd4fc1b28288736767d38926d41612b67
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005731"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Insights](officegraphinsights.md)のプロパティを含む複合型。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
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
| mediaType             | String        | アイテムのメディアの種類。 サポートされている IANA メディア Mime タイプに基づいて、特定の種類のファイルのフィルター処理に使用できます。 すべてのメディア Mime タイプがサポートされるわけではないことに注意してください。 |
| previewImageUrl       | String        | アイテムのプレビューイメージの先頭になる URL。 |
| previewText           | String        | アイテムのプレビューテキスト。 |
| containerWebUrl       | String        | アイテムが格納されるフォルダーへのパス。 |
| containerDisplayName  | String        | アイテムが格納されている場所を示す文字列。 たとえば、SharePoint サイトの名前、またはアイテムを格納している OneDrive の所有者を識別するユーザー名。  |
| containerType         | String | ファイルが格納されているコンテナーの種類によるフィルター処理に使用できます。 サイト、Onedrive Business など。       |

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
-   Project
-   Access
-   メール
-   .Csv
-   アーカイブ
-   Xps
-   オーディオ
-   ビデオ
-   イメージ
-   Web
-   テキスト
-   Xml
-   Story
-   ExternalContent
-   フォルダー
-   Other

クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>containerType プロパティの値
サポートされている種類は、 [Officegraphinsights](officegraphinsights.md)がファイルを返すコンテナーによって異なる場合があります。 たとえば、"DropBox"、"Box"、および "GDrive" からファイルを取得するのは、 [sharepoint](insights-shared.md)のファイルです。

-   Onedrive Business
-   Site
-   メール
-   DropBox
-   検索ボックス
-   GDrive

クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
