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
# <a name="notebook-resource-type"></a><span data-ttu-id="4ca16-103">ノートブックリソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ca16-103">notebook resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ca16-104">OneNote ノートブック。</span><span class="sxs-lookup"><span data-stu-id="4ca16-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ca16-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ca16-105">JSON representation</span></span>

<span data-ttu-id="4ca16-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4ca16-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="4ca16-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ca16-107">Properties</span></span>
| <span data-ttu-id="4ca16-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ca16-108">Property</span></span>     | <span data-ttu-id="4ca16-109">型</span><span class="sxs-lookup"><span data-stu-id="4ca16-109">Type</span></span>   |<span data-ttu-id="4ca16-110">説明</span><span class="sxs-lookup"><span data-stu-id="4ca16-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ca16-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="4ca16-111">createdBy</span></span>|[<span data-ttu-id="4ca16-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="4ca16-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="4ca16-p101">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="4ca16-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ca16-115">createdDateTime</span></span>|<span data-ttu-id="4ca16-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ca16-116">DateTimeOffset</span></span>|<span data-ttu-id="4ca16-117">ノートブックが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4ca16-117">The date and time when the notebook was created.</span></span> <span data-ttu-id="4ca16-118">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4ca16-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4ca16-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4ca16-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-120">Read-only.</span></span>|
|<span data-ttu-id="4ca16-121">id</span><span class="sxs-lookup"><span data-stu-id="4ca16-121">id</span></span>|<span data-ttu-id="4ca16-122">String</span><span class="sxs-lookup"><span data-stu-id="4ca16-122">String</span></span>|<span data-ttu-id="4ca16-123">ノートブックの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4ca16-123">The unique identifier of the notebook.</span></span> <span data-ttu-id="4ca16-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-124">Read-only.</span></span>|
|<span data-ttu-id="4ca16-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="4ca16-125">isDefault</span></span>|<span data-ttu-id="4ca16-126">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="4ca16-126">Boolean</span></span>|<span data-ttu-id="4ca16-127">これがユーザーの既定のノートブックであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-127">Indicates whether this is the user's default notebook.</span></span> <span data-ttu-id="4ca16-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-128">Read-only.</span></span>|
|<span data-ttu-id="4ca16-129">isShared</span><span class="sxs-lookup"><span data-stu-id="4ca16-129">isShared</span></span>|<span data-ttu-id="4ca16-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ca16-130">Boolean</span></span>|<span data-ttu-id="4ca16-131">ノートブックが共有されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-131">Indicates whether the notebook is shared.</span></span> <span data-ttu-id="4ca16-132">true の場合、所有者以外のユーザーがノートブックの内容を表示できます。</span><span class="sxs-lookup"><span data-stu-id="4ca16-132">If true, the contents of the notebook can be seen by people other than the owner.</span></span> <span data-ttu-id="4ca16-133">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4ca16-133">Read-only.</span></span>|
|<span data-ttu-id="4ca16-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4ca16-134">lastModifiedBy</span></span>|[<span data-ttu-id="4ca16-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="4ca16-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="4ca16-p106">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="4ca16-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ca16-138">lastModifiedDateTime</span></span>|<span data-ttu-id="4ca16-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ca16-139">DateTimeOffset</span></span>|<span data-ttu-id="4ca16-140">ノートブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4ca16-140">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="4ca16-141">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-141">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4ca16-142">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4ca16-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4ca16-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-143">Read-only.</span></span>|
|<span data-ttu-id="4ca16-144">リンク</span><span class="sxs-lookup"><span data-stu-id="4ca16-144">links</span></span>|[<span data-ttu-id="4ca16-145">NotebookLinks</span><span class="sxs-lookup"><span data-stu-id="4ca16-145">NotebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="4ca16-146">ノートブックを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="4ca16-146">Links for opening the notebook.</span></span> <span data-ttu-id="4ca16-147">リンク`oneNoteClientURL`がインストールされている場合は、OneNote のネイティブクライアントでノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="4ca16-147">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="4ca16-148">`oneNoteWebURL` リンクは、OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="4ca16-148">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="4ca16-149">displayName</span><span class="sxs-lookup"><span data-stu-id="4ca16-149">displayName</span></span>|<span data-ttu-id="4ca16-150">String</span><span class="sxs-lookup"><span data-stu-id="4ca16-150">String</span></span>|<span data-ttu-id="4ca16-151">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="4ca16-151">The name of the notebook.</span></span>|
|<span data-ttu-id="4ca16-152">sectionグループ url</span><span class="sxs-lookup"><span data-stu-id="4ca16-152">sectionGroupsUrl</span></span>|<span data-ttu-id="4ca16-153">String</span><span class="sxs-lookup"><span data-stu-id="4ca16-153">String</span></span>|<span data-ttu-id="4ca16-154">`sectionGroups`ナビゲーションプロパティの URL。これは、ノートブック内のすべてのセクショングループを返します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-154">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook.</span></span> <span data-ttu-id="4ca16-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-155">Read-only.</span></span>|
|<span data-ttu-id="4ca16-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="4ca16-156">sectionsUrl</span></span>|<span data-ttu-id="4ca16-157">String</span><span class="sxs-lookup"><span data-stu-id="4ca16-157">String</span></span>|<span data-ttu-id="4ca16-158">ノートブック内のすべて`sections`のセクションを返すナビゲーションプロパティの URL。</span><span class="sxs-lookup"><span data-stu-id="4ca16-158">The URL for the `sections` navigation property, which returns all the sections in the notebook.</span></span> <span data-ttu-id="4ca16-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-159">Read-only.</span></span>|
|<span data-ttu-id="4ca16-160">self</span><span class="sxs-lookup"><span data-stu-id="4ca16-160">self</span></span>|<span data-ttu-id="4ca16-161">String</span><span class="sxs-lookup"><span data-stu-id="4ca16-161">String</span></span>|<span data-ttu-id="4ca16-162">ノートブックに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="4ca16-162">The endpoint where you can get details about the notebook.</span></span> <span data-ttu-id="4ca16-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-163">Read-only.</span></span>|
|<span data-ttu-id="4ca16-164">userRole</span><span class="sxs-lookup"><span data-stu-id="4ca16-164">userRole</span></span>|<span data-ttu-id="4ca16-165">String</span><span class="sxs-lookup"><span data-stu-id="4ca16-165">String</span></span>|<span data-ttu-id="4ca16-166">可能な値は、`Owner`、`Contributor`、`Reader`、`None` です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-166">Possible values are: `Owner`, `Contributor`, `Reader`, `None`.</span></span> <span data-ttu-id="4ca16-167">owner ノートブックへの所有者レベルのアクセス権を表します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-167">Owner represents owner-level access to the notebook.</span></span> <span data-ttu-id="4ca16-168">共同作成者は、ノートブックへの読み取り/書き込みアクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-168">Contributor represents read/write access to the notebook.</span></span> <span data-ttu-id="4ca16-169">閲覧者は、ノートブックへの読み取り専用アクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-169">Reader represents read-only access to the notebook.</span></span> <span data-ttu-id="4ca16-170">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-170">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ca16-171">関係</span><span class="sxs-lookup"><span data-stu-id="4ca16-171">Relationships</span></span>
| <span data-ttu-id="4ca16-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ca16-172">Relationship</span></span> | <span data-ttu-id="4ca16-173">型</span><span class="sxs-lookup"><span data-stu-id="4ca16-173">Type</span></span>   |<span data-ttu-id="4ca16-174">説明</span><span class="sxs-lookup"><span data-stu-id="4ca16-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ca16-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="4ca16-175">sectionGroups</span></span>|<span data-ttu-id="4ca16-176">[SectionGroup](sectiongroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4ca16-176">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="4ca16-177">ノートブック内のセクション グループ。</span><span class="sxs-lookup"><span data-stu-id="4ca16-177">The section groups in the notebook.</span></span> <span data-ttu-id="4ca16-178">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-178">Read-only.</span></span> <span data-ttu-id="4ca16-179">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4ca16-179">Nullable.</span></span>|
|<span data-ttu-id="4ca16-180">sections</span><span class="sxs-lookup"><span data-stu-id="4ca16-180">sections</span></span>|<span data-ttu-id="4ca16-181">[Section](section.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4ca16-181">[Section](section.md) collection</span></span>|<span data-ttu-id="4ca16-182">ノートブックのセクション。</span><span class="sxs-lookup"><span data-stu-id="4ca16-182">The sections in the notebook.</span></span> <span data-ttu-id="4ca16-183">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4ca16-183">Read-only.</span></span> <span data-ttu-id="4ca16-184">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4ca16-184">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="4ca16-185">メソッド</span><span class="sxs-lookup"><span data-stu-id="4ca16-185">Methods</span></span>

| <span data-ttu-id="4ca16-186">メソッド</span><span class="sxs-lookup"><span data-stu-id="4ca16-186">Method</span></span>           | <span data-ttu-id="4ca16-187">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4ca16-187">Return Type</span></span>    |<span data-ttu-id="4ca16-188">説明</span><span class="sxs-lookup"><span data-stu-id="4ca16-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ca16-189">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="4ca16-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="4ca16-190">Notebook</span><span class="sxs-lookup"><span data-stu-id="4ca16-190">Notebook</span></span>](notebook.md) |<span data-ttu-id="4ca16-191">ノートブックのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4ca16-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="4ca16-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="4ca16-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="4ca16-193">[recentNotebook](recentnotebook.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4ca16-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="4ca16-194">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="4ca16-195">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="4ca16-195">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="4ca16-196">Notebook</span><span class="sxs-lookup"><span data-stu-id="4ca16-196">Notebook</span></span>](notebook.md) | <span data-ttu-id="4ca16-197">URL パスを使用して、ノートブックオブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-197">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="4ca16-198">セクション グループを作成する</span><span class="sxs-lookup"><span data-stu-id="4ca16-198">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="4ca16-199">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="4ca16-199">SectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="4ca16-200">指定したノートブックの sectiongroups コレクションに投稿して、セクショングループを作成します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-200">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="4ca16-201">セクション グループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4ca16-201">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="4ca16-202">[SectionGroup](sectiongroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4ca16-202">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="4ca16-203">指定されたノートブック内のセクショングループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-203">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="4ca16-204">セクションを作成する</span><span class="sxs-lookup"><span data-stu-id="4ca16-204">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="4ca16-205">Section</span><span class="sxs-lookup"><span data-stu-id="4ca16-205">Section</span></span>](section.md)| <span data-ttu-id="4ca16-206">指定したノートブックの sections コレクションに投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-206">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="4ca16-207">セクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4ca16-207">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="4ca16-208">[Section](section.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4ca16-208">[Section](section.md) collection</span></span>| <span data-ttu-id="4ca16-209">指定されたノートブック内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4ca16-209">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="4ca16-210">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="4ca16-210">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="4ca16-211">なし</span><span class="sxs-lookup"><span data-stu-id="4ca16-211">None</span></span> | <span data-ttu-id="4ca16-212">ノートブックをコピーします。</span><span class="sxs-lookup"><span data-stu-id="4ca16-212">Copies a notebook.</span></span>|

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
