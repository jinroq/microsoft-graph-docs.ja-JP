---
title: page リソースの種類
description: OneNote ノートブックのページ。
localization_priority: Normal
ms.openlocfilehash: d8c27cdc144e9b192bd0205f256653ff7f04df5f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568550"
---
# <a name="page-resource-type"></a>page リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneNote ノートブックのページ。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|content|Stream|ページの HTML コンテンツ。|
|contentUrl|String|ページの HTML コンテンツの URL。  読み取り専用。|
|createdByAppId|String|ページを作成したアプリケーションの一意識別子。 読み取り専用。|
|createdDateTime|DateTimeOffset|ページが作成された日時。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|id|String|ページの一意識別子。  読み取り専用です。|
|lastModifiedDateTime|DateTimeOffset|ページが最後に変更された日付と時刻。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|level|Int32|ページのインデントレベルを示します。 読み取り専用です。|
|リンク|[PageLinks](pagelinks.md)|ページを開くためのリンク。 この`oneNoteClientURL`リンクは、インストールされている場合は、OneNote native client でページを開きます。 この`oneNoteWebUrl`リンクは、OneNote Online でページを開きます。 読み取り専用。|
|降順|Int32|親セクション内のページの順序。 読み取り専用。|
|self|String|ページに関する詳細を取得できるエンドポイント。 読み取り専用。|
|title|String|ページのタイトル。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|ページを含むノートブック。  読み取り専用。|
|parentSection|[Section](section.md)|ページを含むセクション。 値の取得のみ可能です。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ページを取得する](../api/page-get.md) | [Page](page.md) |ページのプロパティとリレーションシップを読み取ります。|
|[ページ コンテンツを更新する](../api/page-update.md) | なし |ページの HTML コンテンツを更新します。 |
|[ページの削除](../api/page-delete.md) | なし |ページを削除します。 |
|[copyToSection](../api/page-copytosection.md)| なし |ページを特定のセクションにコピーします。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/page.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
