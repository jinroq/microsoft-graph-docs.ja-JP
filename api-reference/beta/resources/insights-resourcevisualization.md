---
title: resourceVisualization リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 9dc2d50a5bc694204317f8c3332263ce5259e2fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575105"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複合型が[officeGraphInsights](insights.md)のプロパティを格納します。

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
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 型          | 説明  |
| -------------         |---------------| -------------|
| タイトル                 | String        | アイテムのタイトルのテキストです。               |
| type              | String        | 項目のメディア ・ タイプ。 特定の種類に基づいて特定のファイルをフィルター処理するために使用できます。 サポートされている型の下を参照してください。 |
| メディアの種類             | String        | 項目のメディア ・ タイプ。 IANA メディアのサポートされている Mime の種類に基づいて、ファイルの特定の種類のフィルター処理に使用できます。 すべてのメディアの Mime タイプがサポートされていることに注意してください。 |
| previewImageUrl       | String        | 先頭のアイテムのプレビュー イメージの URL です。 |
| previewText           | String        | アイテムのプレビュー テキストです。 |
| containerWebUrl       | String        | アイテムが格納されるフォルダーへのパスです。 |
| containerDisplayName  | String        | アイテムを保存する場所を説明する文字列。 たとえば、SharePoint サイト、または項目を格納する OneDrive の所有者を識別するユーザー名の名前です。  |
| コンテナー         | String | ファイルを格納するコンテナーの種類によってフィルター処理するために使用できます。 サイトなど OneDriveBusiness。       |

## <a name="type-property-values"></a>プロパティ値の型
-   PowerPoint
-   Word
-   Excel
-   Pdf
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   プロジェクト
-   Access
-   メール
-   Csv
-   アーカイブ
-   Xps
-   オーディオ
-   ビデオ
-   画像
-   Web
-   テキスト
-   Xml
-   Story
-   ExternalContent
-   フォルダー
-   Other

クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>コンテナーのプロパティの値
サポートされている型が異なりますコンテナーの元となる[情報](insights.md)がファイルを返します。 たとえば、のみ[共有](insights-shared.md)情報を得ることは、'ドロップ ボックス'、'ボックス'、および 'ください' からファイルを返します。

-   OneDriveBusiness
-   Site
-   メール
-   ドロップ ボックス
-   ボックス
-   ください

クエリの例:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
