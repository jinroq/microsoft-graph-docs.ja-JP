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
# <a name="notebook-resource-type"></a><span data-ttu-id="dc1d7-103">notebook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc1d7-103">notebook resource type</span></span>

> <span data-ttu-id="dc1d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc1d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc1d7-106">OneNote ノートブックです。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-106">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc1d7-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc1d7-107">JSON representation</span></span>

<span data-ttu-id="dc1d7-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="dc1d7-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="dc1d7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc1d7-109">Properties</span></span>
| <span data-ttu-id="dc1d7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc1d7-110">Property</span></span>     | <span data-ttu-id="dc1d7-111">種類</span><span class="sxs-lookup"><span data-stu-id="dc1d7-111">Type</span></span>   |<span data-ttu-id="dc1d7-112">説明</span><span class="sxs-lookup"><span data-stu-id="dc1d7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc1d7-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="dc1d7-113">createdBy</span></span>|[<span data-ttu-id="dc1d7-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="dc1d7-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="dc1d7-p102">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1d7-117">createdDateTime</span></span>|<span data-ttu-id="dc1d7-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1d7-118">DateTimeOffset</span></span>|<span data-ttu-id="dc1d7-p103">ノートブックが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p103">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-123">id</span><span class="sxs-lookup"><span data-stu-id="dc1d7-123">id</span></span>|<span data-ttu-id="dc1d7-124">String</span><span class="sxs-lookup"><span data-stu-id="dc1d7-124">String</span></span>|<span data-ttu-id="dc1d7-p104">ノートブックの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p104">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="dc1d7-127">isDefault</span></span>|<span data-ttu-id="dc1d7-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="dc1d7-128">Boolean</span></span>|<span data-ttu-id="dc1d7-p105">これがユーザーの既定のノートブックであるかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p105">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-131">IsShared</span><span class="sxs-lookup"><span data-stu-id="dc1d7-131">isShared</span></span>|<span data-ttu-id="dc1d7-132">ブール型</span><span class="sxs-lookup"><span data-stu-id="dc1d7-132">Boolean</span></span>|<span data-ttu-id="dc1d7-p106">ノートブックを共有するかどうかを示します。True の場合、所有者以外のユーザーにノートブックのコンテンツが表示されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p106">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="dc1d7-136">lastModifiedBy</span></span>|[<span data-ttu-id="dc1d7-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="dc1d7-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="dc1d7-p107">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc1d7-140">lastModifiedDateTime</span></span>|<span data-ttu-id="dc1d7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc1d7-141">DateTimeOffset</span></span>|<span data-ttu-id="dc1d7-p108">ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p108">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-146">links</span><span class="sxs-lookup"><span data-stu-id="dc1d7-146">links</span></span>|[<span data-ttu-id="dc1d7-147">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="dc1d7-147">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="dc1d7-p109">ノートブックを開くためのリンク。`oneNoteClientURL` リンクが OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。`oneNoteWebURL` リンクでは、OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p109">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="dc1d7-151">displayName</span><span class="sxs-lookup"><span data-stu-id="dc1d7-151">displayName</span></span>|<span data-ttu-id="dc1d7-152">String</span><span class="sxs-lookup"><span data-stu-id="dc1d7-152">String</span></span>|<span data-ttu-id="dc1d7-153">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-153">The name of the notebook.</span></span>|
|<span data-ttu-id="dc1d7-154">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="dc1d7-154">sectionGroupsUrl</span></span>|<span data-ttu-id="dc1d7-155">String</span><span class="sxs-lookup"><span data-stu-id="dc1d7-155">String</span></span>|<span data-ttu-id="dc1d7-p110">ノートブック内のすべてのセクション グループを返す `sectionGroups` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p110">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-158">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="dc1d7-158">sectionsUrl</span></span>|<span data-ttu-id="dc1d7-159">String</span><span class="sxs-lookup"><span data-stu-id="dc1d7-159">String</span></span>|<span data-ttu-id="dc1d7-p111">ノートブック内のすべてのセクションを返す `sections` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p111">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-162">self</span><span class="sxs-lookup"><span data-stu-id="dc1d7-162">self</span></span>|<span data-ttu-id="dc1d7-163">String</span><span class="sxs-lookup"><span data-stu-id="dc1d7-163">String</span></span>|<span data-ttu-id="dc1d7-p112">ノートブックに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p112">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="dc1d7-166">userRole</span><span class="sxs-lookup"><span data-stu-id="dc1d7-166">userRole</span></span>|<span data-ttu-id="dc1d7-167">String</span><span class="sxs-lookup"><span data-stu-id="dc1d7-167">String</span></span>|<span data-ttu-id="dc1d7-p113">使用可能な値: `Owner`、`Contributor`、`Reader`、`None`。Owner は、ノートブックへの所有者レベルのアクセス権を表します。Contributor は、ノートブックへの読み取り/書き込みアクセス権を表します。Reader は、ノートブックへの読み取り専用アクセス権を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p113">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc1d7-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc1d7-173">Relationships</span></span>
| <span data-ttu-id="dc1d7-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dc1d7-174">Relationship</span></span> | <span data-ttu-id="dc1d7-175">型</span><span class="sxs-lookup"><span data-stu-id="dc1d7-175">Type</span></span>   |<span data-ttu-id="dc1d7-176">説明</span><span class="sxs-lookup"><span data-stu-id="dc1d7-176">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc1d7-177">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="dc1d7-177">sectionGroups</span></span>|<span data-ttu-id="dc1d7-178">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc1d7-178">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="dc1d7-p114">ノートブック内のセクション グループ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p114">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="dc1d7-182">sections</span><span class="sxs-lookup"><span data-stu-id="dc1d7-182">sections</span></span>|<span data-ttu-id="dc1d7-183">[Section](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc1d7-183">[Section](section.md) collection</span></span>|<span data-ttu-id="dc1d7-p115">ノートブック内のセクション。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-p115">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="dc1d7-187">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc1d7-187">Methods</span></span>

| <span data-ttu-id="dc1d7-188">メソッド</span><span class="sxs-lookup"><span data-stu-id="dc1d7-188">Method</span></span>           | <span data-ttu-id="dc1d7-189">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dc1d7-189">Return Type</span></span>    |<span data-ttu-id="dc1d7-190">説明</span><span class="sxs-lookup"><span data-stu-id="dc1d7-190">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc1d7-191">Get notebook</span><span class="sxs-lookup"><span data-stu-id="dc1d7-191">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="dc1d7-192">Notebook</span><span class="sxs-lookup"><span data-stu-id="dc1d7-192">Notebook</span></span>](notebook.md) |<span data-ttu-id="dc1d7-193">ノートブックのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-193">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="dc1d7-194">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="dc1d7-194">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="dc1d7-195">[recentNotebook](recentnotebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc1d7-195">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="dc1d7-196">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-196">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="dc1d7-197">Create section group</span><span class="sxs-lookup"><span data-stu-id="dc1d7-197">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="dc1d7-198">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="dc1d7-198">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="dc1d7-199">指定したノートブックで sectionGroup コレクションに投稿してセクション グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-199">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="dc1d7-200">List section groups</span><span class="sxs-lookup"><span data-stu-id="dc1d7-200">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="dc1d7-201">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc1d7-201">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="dc1d7-202">指定されたノートブック内のセクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-202">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="dc1d7-203">Create section</span><span class="sxs-lookup"><span data-stu-id="dc1d7-203">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="dc1d7-204">Section</span><span class="sxs-lookup"><span data-stu-id="dc1d7-204">Section</span></span>](section.md)| <span data-ttu-id="dc1d7-205">指定されたノートブックでセクションのコレクションに投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-205">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="dc1d7-206">List sections</span><span class="sxs-lookup"><span data-stu-id="dc1d7-206">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="dc1d7-207">[Section](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc1d7-207">[Section](section.md) collection</span></span>| <span data-ttu-id="dc1d7-208">指定されたノートブック内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-208">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="dc1d7-209">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="dc1d7-209">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="dc1d7-210">なし</span><span class="sxs-lookup"><span data-stu-id="dc1d7-210">None</span></span> | <span data-ttu-id="dc1d7-211">ノートブックをコピーします。</span><span class="sxs-lookup"><span data-stu-id="dc1d7-211">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
