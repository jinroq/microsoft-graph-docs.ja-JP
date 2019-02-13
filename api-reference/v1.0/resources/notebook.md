---
title: notebook リソースの種類
description: OneNote ノートブックです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 96be6a41424260610794f9a0df4ef8e35dc1597f
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967334"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="53afa-103">notebook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="53afa-103">notebook resource type</span></span>

<span data-ttu-id="53afa-104">OneNote ノートブックです。</span><span class="sxs-lookup"><span data-stu-id="53afa-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53afa-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="53afa-105">JSON representation</span></span>

<span data-ttu-id="53afa-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="53afa-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
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
## <a name="properties"></a><span data-ttu-id="53afa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53afa-107">Properties</span></span>
| <span data-ttu-id="53afa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53afa-108">Property</span></span>     | <span data-ttu-id="53afa-109">型</span><span class="sxs-lookup"><span data-stu-id="53afa-109">Type</span></span>   |<span data-ttu-id="53afa-110">説明</span><span class="sxs-lookup"><span data-stu-id="53afa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53afa-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="53afa-111">createdBy</span></span>|[<span data-ttu-id="53afa-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="53afa-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="53afa-p101">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="53afa-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="53afa-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53afa-115">createdDateTime</span></span>|<span data-ttu-id="53afa-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53afa-116">DateTimeOffset</span></span>|<span data-ttu-id="53afa-p102">ノートブックが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p102">The date and time when the notebook was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="53afa-121">id</span><span class="sxs-lookup"><span data-stu-id="53afa-121">id</span></span>|<span data-ttu-id="53afa-122">文字列</span><span class="sxs-lookup"><span data-stu-id="53afa-122">String</span></span>|<span data-ttu-id="53afa-p103">ノートブックの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p103">The unique identifier of the notebook. Read-only.</span></span>|
|<span data-ttu-id="53afa-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="53afa-125">isDefault</span></span>|<span data-ttu-id="53afa-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="53afa-126">Boolean</span></span>|<span data-ttu-id="53afa-p104">これがユーザーの既定のノートブックであるかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p104">Indicates whether this is the user's default notebook. Read-only.</span></span>|
|<span data-ttu-id="53afa-129">IsShared</span><span class="sxs-lookup"><span data-stu-id="53afa-129">isShared</span></span>|<span data-ttu-id="53afa-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="53afa-130">Boolean</span></span>|<span data-ttu-id="53afa-p105">ノートブックを共有するかどうかを示します。True の場合、所有者以外のユーザーにノートブックのコンテンツが表示されます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p105">Indicates whether the notebook is shared. If true, the contents of the notebook can be seen by people other than the owner. Read-only.</span></span>|
|<span data-ttu-id="53afa-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="53afa-134">lastModifiedBy</span></span>|[<span data-ttu-id="53afa-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="53afa-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="53afa-p106">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="53afa-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53afa-138">lastModifiedDateTime</span></span>|<span data-ttu-id="53afa-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53afa-139">DateTimeOffset</span></span>|<span data-ttu-id="53afa-p107">ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p107">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="53afa-144">links</span><span class="sxs-lookup"><span data-stu-id="53afa-144">links</span></span>|[<span data-ttu-id="53afa-145">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="53afa-145">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="53afa-p108">ノートブックを開くためのリンク。`oneNoteClientURL` リンクが OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。`oneNoteWebURL` リンクでは、OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="53afa-p108">Links for opening the notebook. The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="53afa-149">displayName</span><span class="sxs-lookup"><span data-stu-id="53afa-149">displayName</span></span>|<span data-ttu-id="53afa-150">String</span><span class="sxs-lookup"><span data-stu-id="53afa-150">String</span></span>|<span data-ttu-id="53afa-151">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="53afa-151">The name of the notebook.</span></span>|
|<span data-ttu-id="53afa-152">sectionGroupsUrl</span><span class="sxs-lookup"><span data-stu-id="53afa-152">sectionGroupsUrl</span></span>|<span data-ttu-id="53afa-153">String</span><span class="sxs-lookup"><span data-stu-id="53afa-153">String</span></span>|<span data-ttu-id="53afa-p109">ノートブック内のすべてのセクション グループを返す `sectionGroups` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p109">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook. Read-only.</span></span>|
|<span data-ttu-id="53afa-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="53afa-156">sectionsUrl</span></span>|<span data-ttu-id="53afa-157">String</span><span class="sxs-lookup"><span data-stu-id="53afa-157">String</span></span>|<span data-ttu-id="53afa-p110">ノートブック内のすべてのセクションを返す `sections` ナビゲーション プロパティの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p110">The URL for the `sections` navigation property, which returns all the sections in the notebook. Read-only.</span></span>|
|<span data-ttu-id="53afa-160">self</span><span class="sxs-lookup"><span data-stu-id="53afa-160">self</span></span>|<span data-ttu-id="53afa-161">String</span><span class="sxs-lookup"><span data-stu-id="53afa-161">String</span></span>|<span data-ttu-id="53afa-p111">ノートブックに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p111">The endpoint where you can get details about the notebook. Read-only.</span></span>|
|<span data-ttu-id="53afa-164">userRole</span><span class="sxs-lookup"><span data-stu-id="53afa-164">userRole</span></span>|<span data-ttu-id="53afa-165">onenoteUserRole</span><span class="sxs-lookup"><span data-stu-id="53afa-165">onenoteUserRole</span></span>|<span data-ttu-id="53afa-p112">使用可能な値: `Owner`、`Contributor`、`Reader`、`None`。Owner は、ノートブックへの所有者レベルのアクセス権を表します。Contributor は、ノートブックへの読み取り/書き込みアクセス権を表します。Reader は、ノートブックへの読み取り専用アクセス権を表します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53afa-p112">Possible values are: `Owner`, `Contributor`, `Reader`, `None`. Owner represents owner-level access to the notebook. Contributor represents read/write access to the notebook. Reader represents read-only access to the notebook. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53afa-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="53afa-171">Relationships</span></span>
| <span data-ttu-id="53afa-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="53afa-172">Relationship</span></span> | <span data-ttu-id="53afa-173">型</span><span class="sxs-lookup"><span data-stu-id="53afa-173">Type</span></span>   |<span data-ttu-id="53afa-174">説明</span><span class="sxs-lookup"><span data-stu-id="53afa-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53afa-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="53afa-175">sectionGroups</span></span>|<span data-ttu-id="53afa-176">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="53afa-176">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="53afa-p113">ノートブック内のセクション グループ。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="53afa-p113">The section groups in the notebook. Read-only. Nullable.</span></span>|
|<span data-ttu-id="53afa-180">sections</span><span class="sxs-lookup"><span data-stu-id="53afa-180">sections</span></span>|<span data-ttu-id="53afa-181">[OnenoteSection](section.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="53afa-181">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="53afa-p114">ノートブック内のセクション。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="53afa-p114">The sections in the notebook. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="53afa-185">メソッド</span><span class="sxs-lookup"><span data-stu-id="53afa-185">Methods</span></span>

| <span data-ttu-id="53afa-186">メソッド</span><span class="sxs-lookup"><span data-stu-id="53afa-186">Method</span></span>           | <span data-ttu-id="53afa-187">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="53afa-187">Return Type</span></span>    |<span data-ttu-id="53afa-188">説明</span><span class="sxs-lookup"><span data-stu-id="53afa-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53afa-189">Get notebook</span><span class="sxs-lookup"><span data-stu-id="53afa-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="53afa-190">Notebook</span><span class="sxs-lookup"><span data-stu-id="53afa-190">Notebook</span></span>](notebook.md) |<span data-ttu-id="53afa-191">ノートブックのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="53afa-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="53afa-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="53afa-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="53afa-193">[recentNotebook](recentnotebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="53afa-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="53afa-194">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="53afa-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="53afa-195">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="53afa-195">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="53afa-196">Notebook</span><span class="sxs-lookup"><span data-stu-id="53afa-196">Notebook</span></span>](notebook.md) | <span data-ttu-id="53afa-197">プロパティと URL パスを使用してノートブックのオブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="53afa-197">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="53afa-198">Create section group</span><span class="sxs-lookup"><span data-stu-id="53afa-198">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="53afa-199">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="53afa-199">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="53afa-200">指定したノートブックで sectionGroup コレクションに投稿してセクション グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="53afa-200">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="53afa-201">List section groups</span><span class="sxs-lookup"><span data-stu-id="53afa-201">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="53afa-202">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="53afa-202">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="53afa-203">指定されたノートブック内のセクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="53afa-203">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="53afa-204">Create section</span><span class="sxs-lookup"><span data-stu-id="53afa-204">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="53afa-205">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="53afa-205">OnenoteSection</span></span>](section.md)| <span data-ttu-id="53afa-206">指定されたノートブックでセクションのコレクションに投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="53afa-206">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="53afa-207">List sections</span><span class="sxs-lookup"><span data-stu-id="53afa-207">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="53afa-208">[OnenoteSection](section.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="53afa-208">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="53afa-209">指定されたノートブック内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="53afa-209">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="53afa-210">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="53afa-210">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="53afa-211">なし</span><span class="sxs-lookup"><span data-stu-id="53afa-211">None</span></span> | <span data-ttu-id="53afa-212">ノートブックをコピーします。</span><span class="sxs-lookup"><span data-stu-id="53afa-212">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
