---
title: ノートブックリソースの種類
description: OneNote ノートブック。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 24e9a7a4b87a59af27166121aff2847f5f15d894
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459130"
---
# <a name="notebook-resource-type"></a>ノートブックリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OneNote ノートブック。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|createdDateTime|DateTimeOffset|ノートブックが作成された日時。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|id|String|ノートブックの一意識別子。 読み取り専用です。|
|isDefault|ブール型 (Boolean)|これがユーザーの既定のノートブックであるかどうかを示します。 読み取り専用です。|
|isShared|Boolean|ノートブックが共有されているかどうかを示します。 true の場合、所有者以外のユーザーがノートブックの内容を表示できます。 読み取り専用。|
|lastModifiedBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|lastModifiedDateTime|DateTimeOffset|ノートブックが最後に変更された日時。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。|
|リンク|[NotebookLinks](notebooklinks.md)|ノートブックを開くためのリンク。 リンク`oneNoteClientURL`がインストールされている場合は、OneNote のネイティブクライアントでノートブックを開きます。 `oneNoteWebURL` リンクは、OneNote Online でノートブックを開きます。|
|displayName|String|ノートブックの名前。|
|sectionグループ url|String|`sectionGroups`ナビゲーションプロパティの URL。これは、ノートブック内のすべてのセクショングループを返します。 読み取り専用です。|
|sectionsUrl|String|ノートブック内のすべて`sections`のセクションを返すナビゲーションプロパティの URL。 読み取り専用です。|
|self|String|ノートブックに関する詳細を取得できるエンドポイント。 読み取り専用です。|
|userRole|String|可能な値は、`Owner`、`Contributor`、`Reader`、`None` です。 owner ノートブックへの所有者レベルのアクセス権を表します。 共同作成者は、ノートブックへの読み取り/書き込みアクセスを表します。 閲覧者は、ノートブックへの読み取り専用アクセスを表します。 読み取り専用です。|

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|sectionGroups|[SectionGroup](sectiongroup.md)コレクション|ノートブック内のセクション グループ。 読み取り専用です。 Null 許容型。|
|sections|[Section](section.md)コレクション|ノートブックのセクション。 読み取り専用です。 Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[ノートブックを取得する](../api/notebook-get.md) | [Notebook](notebook.md) |ノートブックのプロパティとリレーションシップを読み取ります。|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | [recentNotebook](recentnotebook.md)コレクション | ユーザーの最近アクセスしたノートブックのコレクションを取得します。 |
|[getNotebookFromWebUrl](../api/notebook-getnotebookfromweburl.md) | [Notebook](notebook.md) | URL パスを使用して、ノートブックオブジェクトのプロパティとリレーションシップを取得します。 |
|[セクション グループを作成する](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| 指定したノートブックの sectiongroups コレクションに投稿して、セクショングループを作成します。|
|[セクション グループを一覧表示する](../api/notebook-list-sectiongroups.md) |[SectionGroup](sectiongroup.md)コレクション| 指定されたノートブック内のセクショングループのコレクションを取得します。|
|[セクションを作成する](../api/notebook-post-sections.md) |[Section](section.md)| 指定したノートブックの sections コレクションに投稿してセクションを作成します。|
|[セクションを一覧表示する](../api/notebook-list-sections.md) |[Section](section.md)コレクション| 指定されたノートブック内のセクションのコレクションを取得します。|
|[copyNotebook](../api/notebook-copynotebook.md)| なし | ノートブックをコピーします。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/notebook.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
