---
title: notebook リソースの種類
description: OneNote ノートブックです。
author: Jewan-microsoft
ms.openlocfilehash: b6301e53d1cc616897055df0185601400f87de54
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362217"
---
# <a name="notebook-resource-type"></a>notebook リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

OneNote ノートブックです。

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
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|createdDateTime|DateTimeOffset|ノートブックが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|
|id|String|ノートブックの一意識別子。読み取り専用です。|
|isDefault|ブール型|これがユーザーの既定のノートブックであるかどうかを示します。読み取り専用です。|
|IsShared|ブール型|ノートブックを共有するかどうかを示します。True の場合、所有者以外のユーザーにノートブックのコンテンツが表示されます。読み取り専用です。|
|lastModifiedBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|lastModifiedDateTime|DateTimeOffset|ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|
|links|[NotebookLinks](notebooklinks.md)|ノートブックを開くためのリンク。`oneNoteClientURL` リンクが OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。`oneNoteWebURL` リンクでは、OneNote Online でノートブックを開きます。|
|displayName|String|ノートブックの名前。|
|sectionGroupsUrl|String|ノートブック内のすべてのセクション グループを返す `sectionGroups` ナビゲーション プロパティの URL。読み取り専用です。|
|sectionsUrl|String|ノートブック内のすべてのセクションを返す `sections` ナビゲーション プロパティの URL。読み取り専用です。|
|self|String|ノートブックに関する詳細情報を入手できるエンドポイント。読み取り専用です。|
|userRole|String|使用可能な値: `Owner`、`Contributor`、`Reader`、`None`。Owner は、ノートブックへの所有者レベルのアクセス権を表します。Contributor は、ノートブックへの読み取り/書き込みアクセス権を表します。Reader は、ノートブックへの読み取り専用アクセス権を表します。読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|sectionGroups|[SectionGroup](sectiongroup.md) コレクション|ノートブック内のセクション グループ。読み取り専用です。Null 許容型。|
|sections|[Section](section.md) コレクション|ノートブック内のセクション。読み取り専用です。Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[Get notebook](../api/notebook-get.md) | [Notebook](notebook.md) |ノートブックのプロパティとリレーションシップを読み取ります。|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | [recentNotebook](recentnotebook.md) コレクション | ユーザーの最近アクセスしたノートブックのコレクションを取得します。 |
|[Create section group](../api/notebook-post-sectiongroups.md) |[SectionGroup](sectiongroup.md)| 指定したノートブックで sectionGroup コレクションに投稿してセクション グループを作成します。|
|[List section groups](../api/notebook-list-sectiongroups.md) |[SectionGroup](sectiongroup.md) コレクション| 指定されたノートブック内のセクション グループのコレクションを取得します。|
|[Create section](../api/notebook-post-sections.md) |[Section](section.md)| 指定されたノートブックでセクションのコレクションに投稿してセクションを作成します。|
|[List sections](../api/notebook-list-sections.md) |[Section](section.md) コレクション| 指定されたノートブック内のセクションのコレクションを取得します。|
|[copyNotebook](../api/notebook-copynotebook.md)| なし | ノートブックをコピーします。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
