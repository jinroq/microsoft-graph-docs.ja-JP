---
title: セクションリソースの種類
description: OneNote ノートブックのセクション。 セクションには、ページを含めることができます。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3246cd861d61130ea83ab8a02886a9f281603398
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034567"
---
# <a name="section-resource-type"></a>セクションリソースの種類

OneNote ノートブックのセクション。 セクションには、ページを含めることができます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "optionalProperties": [
    "pages",
    "parentNotebook",
    "parentSectionGroup"
  ],
  "@odata.type": "microsoft.graph.onenoteSection"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.sectionLinks"},
  "displayName": "string",
  "pagesUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|createdDateTime|DateTimeOffset|セクションが作成された日時。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|id|文字列|セクションの一意識別子。  読み取り専用です。|
|isDefault|ブール型 (Boolean)|これがユーザーの既定のセクションであるかどうかを示します。 読み取り専用です。|
|lastModifiedBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|lastModifiedDateTime|DateTimeOffset|セクションが最後に変更された日時。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|リンク|[SectionLinks](sectionlinks.md)|セクションを開くためのリンク。 リンク`oneNoteClientURL`によって、OneNote native client のセクションがインストールされている場合は、そのセクションが開きます。 リンク`oneNoteWebURL`は、web 上の OneNote でセクションを開きます。|
|displayName|String|セクションの名前。 |
|pagesUrl|String|セクション`pages`内のすべてのページの詳細を取得できるエンドポイント。 読み取り専用です。|
|self|String|セクションに関する詳細を取得できるエンドポイント。 読み取り専用。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|ページ|[OnenotePage](page.md)コレクション|セクション内のページのコレクションです。  読み取り専用です。 Null 許容型。|
|parentNotebook|[Notebook](notebook.md)|セクションを含むノートブック。  読み取り専用です。|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|セクションを含むセクショングループ。  値の取得のみ可能です。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[セクションを取得する](../api/section-get.md) | [OnenoteSection](section.md) |セクションのプロパティとリレーションシップを読み取ります。|
|[Create page](../api/section-post-pages.md) |[Page](page.md)| 指定したセクションの pages コレクションへの投稿によってページを作成します。|
|[List pages](../api/section-list-pages.md) |[Page](page.md) collection| 指定したセクション内のページのコレクションを取得します。|
|[copyToNotebook](../api/section-copytonotebook.md)|None|セクションを特定のノートブックにコピーします。|
|[copyToSectionGroup](../api/section-copytosectiongroup.md)|None|セクションを特定のセクショングループにコピーします。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
