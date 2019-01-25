---
title: resourceVisualization リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526761"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複合型のプロパティ[情報](insights.md)にはが含まれています。

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
| タイトル                 | String        | アイテムのタイトルのテキストです。               |
| type              | String        | 項目のメディア ・ タイプ。 特定の種類に基づいて特定のファイルをフィルター処理するために使用できます。 サポートされている型の下を参照してください。 |
| MediaType             | String        | 項目のメディア ・ タイプ。 IANA メディアのサポートされている Mime の種類に基づいて、ファイルの特定の種類のフィルター処理に使用できます。 すべてのメディアの Mime タイプがサポートされていることに注意してください。 |
| PreviewImageUrl       | String        | 先頭のアイテムのプレビュー イメージの URL です。 |
| previewText           | String        | アイテムのプレビュー テキストです。 |
| containerWebUrl       | String        | アイテムが格納されるフォルダーへのパスです。 |
| containerDisplayName  | String        | アイテムを保存する場所を説明する文字列。 たとえば、SharePoint サイト、または項目を格納する OneDrive の所有者を識別するユーザー名の名前です。  |
| ContainerType         | String | ファイルを格納するコンテナーの種類によってフィルター処理するために使用できます。 サイトなど OneDriveBusiness。       |

## <a name="type-property-values"></a>プロパティ値の型
-   PowerPoint
-   Word
-   Excel
-   PDF
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Access
-   メール
-   *.csv
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
-   Dropbox
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
