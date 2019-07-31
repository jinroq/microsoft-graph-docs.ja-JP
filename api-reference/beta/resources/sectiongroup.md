---
title: sectionGroup リソースの種類
description: OneNote ノートブックのセクショングループ。 セクショングループには、セクションとセクショングループを含めることができます。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 4637784ac20d92c82e7a4771c815136ddd3e175a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965272"
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
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sectionGroup"
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
|id|文字列|セクション グループの一意識別子。 読み取り専用。|
|lastModifiedBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|lastModifiedDateTime|DateTimeOffset|セクション グループが最後に変更された日時。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|displayName|String|セクション グループの名前。|
|Sectionグループ Url|String|`sectionGroups`ナビゲーションプロパティの URL。セクショングループ内のすべてのセクショングループを返します。 読み取り専用です。|
|sectionsUrl|String|`sections`ナビゲーションプロパティの URL。セクショングループ内のすべてのセクションを返します。 読み取り専用です。|
|self|String|セクション グループに関する詳細を取得できるエンドポイント。 読み取り専用。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|parentNotebook|[ノートブック](notebook.md)|セクショングループを含むノートブック。 読み取り専用です。|
|parentSectionGroup|[sectionGroup](sectiongroup.md)|セクショングループを含むセクショングループ。 読み取り専用です。|
|sectionGroups|[sectionGroup](sectiongroup.md)コレクション|セクション内のセクショングループ。 読み取り専用です。 Null 許容型。|
|セクション|[onenoteSection](onenotesection.md)コレクション|セクショングループ内のセクション。 読み取り専用です。 Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[セクション グループを取得する](../api/sectiongroup-get.md) | [sectionGroup](sectiongroup.md) |セクショングループのプロパティとリレーションシップを読み取ります。|
|[セクション グループを作成する](../api/sectiongroup-post-sectiongroups.md) |[sectionGroup](sectiongroup.md)| 指定したセクショングループの sectionGroups コレクションに投稿して、セクショングループを作成します。|
|[List section groups](../api/sectiongroup-list-sectiongroups.md) |[sectionGroup](sectiongroup.md)コレクション| 指定したセクショングループ内のセクショングループのコレクションを取得します。|
|[セクションを作成する](../api/sectiongroup-post-sections.md) |[onenoteSection](onenotesection.md)| 指定したセクショングループ内の sections コレクションに投稿してセクションを作成します。|
|[List sections](../api/sectiongroup-list-sections.md) |[onenoteSection](onenotesection.md)コレクション| 指定したセクショングループ内のセクションのコレクションを取得します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
