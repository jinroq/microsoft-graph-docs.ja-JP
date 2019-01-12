---
title: resourceVisualization リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8426d13968e5bea929c8e26f71346fa554a5242
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990657"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
-   Project
-   Access
-   メール
-   Csv
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
-   その他

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
