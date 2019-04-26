---
title: sectionGroup リソースの種類
description: OneNote ノートブックのセクショングループ。 セクショングループには、セクションとセクショングループを含めることができます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 65e420d014add658a538deb42c01518cd94d611c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562889"
---
# <a name="sectiongroup-resource-type"></a>sectionGroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneNote ノートブックのセクショングループ。 セクショングループには、セクションとセクショングループを含めることができます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSectionGroup",
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.sectiongroup"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|createdDateTime|DateTimeOffset|セクション グループが作成された日時。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|id|String|セクション グループの一意識別子。 読み取り専用。|
|lastModifiedBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|lastModifiedDateTime|DateTimeOffset|セクション グループが最後に変更された日時。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|displayName|String|セクション グループの名前。|
|sectionグループ url|String|`sectionGroups`ナビゲーションプロパティの URL。セクショングループ内のすべてのセクショングループを返します。 読み取り専用。|
|sectionsUrl|String|`sections`ナビゲーションプロパティの URL。セクショングループ内のすべてのセクションを返します。 読み取り専用。|
|self|String|セクション グループに関する詳細を取得できるエンドポイント。 読み取り専用。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|parentNotebook|[Notebook](notebook.md)|セクショングループを含むノートブック。 読み取り専用です。|
|parentSectionGroup|[SectionGroup](sectiongroup.md)|セクショングループを含むセクショングループ。 読み取り専用。|
|sectionGroups|[SectionGroup](sectiongroup.md) collection|セクション内のセクショングループ。 読み取り専用。 Null 許容型。|
|セクション|[Section](section.md)コレクション|セクショングループ内のセクション。 読み取り専用。 Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[セクション グループを取得する](../api/sectiongroup-get.md) | [SectionGroup](sectiongroup.md) |セクショングループのプロパティとリレーションシップを読み取ります。|
|[セクション グループを作成する](../api/sectiongroup-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| 指定したセクショングループの sectiongroups コレクションに投稿して、セクショングループを作成します。|
|[List section groups](../api/sectiongroup-list-sectiongroups.md) |[SectionGroup](sectiongroup.md) collection| 指定したセクショングループ内のセクショングループのコレクションを取得します。|
|[セクションを作成する](../api/sectiongroup-post-sections.md) |[Section](section.md)| 指定したセクショングループ内の sections コレクションに投稿してセクションを作成します。|
|[List sections](../api/sectiongroup-list-sections.md) |[Section](section.md)コレクション| 指定したセクショングループ内のセクションのコレクションを取得します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sectiongroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
