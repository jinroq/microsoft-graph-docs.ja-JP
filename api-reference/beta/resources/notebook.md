---
title: ノートブックリソースの種類
description: OneNote ノートブック。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: e63a03b679460f318747f2a81dac9aa859746a9f
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236637"
---
# <a name="notebook-resource-type"></a><span data-ttu-id="699be-103">ノートブックリソースの種類</span><span class="sxs-lookup"><span data-stu-id="699be-103">notebook resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="699be-104">OneNote ノートブック。</span><span class="sxs-lookup"><span data-stu-id="699be-104">A OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="699be-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="699be-105">JSON representation</span></span>

<span data-ttu-id="699be-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="699be-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
## <a name="properties"></a><span data-ttu-id="699be-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="699be-107">Properties</span></span>
| <span data-ttu-id="699be-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="699be-108">Property</span></span>     | <span data-ttu-id="699be-109">型</span><span class="sxs-lookup"><span data-stu-id="699be-109">Type</span></span>   |<span data-ttu-id="699be-110">説明</span><span class="sxs-lookup"><span data-stu-id="699be-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="699be-111">createdBy</span><span class="sxs-lookup"><span data-stu-id="699be-111">createdBy</span></span>|[<span data-ttu-id="699be-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="699be-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="699be-p101">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-p101">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="699be-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="699be-115">createdDateTime</span></span>|<span data-ttu-id="699be-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="699be-116">DateTimeOffset</span></span>|<span data-ttu-id="699be-117">ノートブックが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="699be-117">The date and time when the notebook was created.</span></span> <span data-ttu-id="699be-118">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="699be-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="699be-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="699be-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="699be-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-120">Read-only.</span></span>|
|<span data-ttu-id="699be-121">id</span><span class="sxs-lookup"><span data-stu-id="699be-121">id</span></span>|<span data-ttu-id="699be-122">文字列</span><span class="sxs-lookup"><span data-stu-id="699be-122">String</span></span>|<span data-ttu-id="699be-123">ノートブックの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="699be-123">The unique identifier of the notebook.</span></span> <span data-ttu-id="699be-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-124">Read-only.</span></span>|
|<span data-ttu-id="699be-125">isDefault</span><span class="sxs-lookup"><span data-stu-id="699be-125">isDefault</span></span>|<span data-ttu-id="699be-126">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="699be-126">Boolean</span></span>|<span data-ttu-id="699be-127">これがユーザーの既定のノートブックであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="699be-127">Indicates whether this is the user's default notebook.</span></span> <span data-ttu-id="699be-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-128">Read-only.</span></span>|
|<span data-ttu-id="699be-129">isShared</span><span class="sxs-lookup"><span data-stu-id="699be-129">isShared</span></span>|<span data-ttu-id="699be-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="699be-130">Boolean</span></span>|<span data-ttu-id="699be-131">ノートブックが共有されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="699be-131">Indicates whether the notebook is shared.</span></span> <span data-ttu-id="699be-132">true の場合、所有者以外のユーザーがノートブックの内容を表示できます。</span><span class="sxs-lookup"><span data-stu-id="699be-132">If true, the contents of the notebook can be seen by people other than the owner.</span></span> <span data-ttu-id="699be-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-133">Read-only.</span></span>|
|<span data-ttu-id="699be-134">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="699be-134">lastModifiedBy</span></span>|[<span data-ttu-id="699be-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="699be-135">identitySet</span></span>](identityset.md)|<span data-ttu-id="699be-p106">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-p106">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="699be-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="699be-138">lastModifiedDateTime</span></span>|<span data-ttu-id="699be-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="699be-139">DateTimeOffset</span></span>|<span data-ttu-id="699be-140">ノートブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="699be-140">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="699be-141">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="699be-141">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="699be-142">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="699be-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="699be-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-143">Read-only.</span></span>|
|<span data-ttu-id="699be-144">リンク</span><span class="sxs-lookup"><span data-stu-id="699be-144">links</span></span>|[<span data-ttu-id="699be-145">notebookLinks</span><span class="sxs-lookup"><span data-stu-id="699be-145">notebookLinks</span></span>](notebooklinks.md)|<span data-ttu-id="699be-146">ノートブックを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="699be-146">Links for opening the notebook.</span></span> <span data-ttu-id="699be-147">リンク`oneNoteClientURL`がインストールされている場合は、OneNote のネイティブクライアントでノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="699be-147">The `oneNoteClientURL` link opens the notebook in the OneNote native client if it's installed.</span></span> <span data-ttu-id="699be-148">リンク`oneNoteWebURL`は、OneNote で web 上のノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="699be-148">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="699be-149">displayName</span><span class="sxs-lookup"><span data-stu-id="699be-149">displayName</span></span>|<span data-ttu-id="699be-150">String</span><span class="sxs-lookup"><span data-stu-id="699be-150">String</span></span>|<span data-ttu-id="699be-151">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="699be-151">The name of the notebook.</span></span>|
|<span data-ttu-id="699be-152">Sectionグループ Url</span><span class="sxs-lookup"><span data-stu-id="699be-152">sectionGroupsUrl</span></span>|<span data-ttu-id="699be-153">String</span><span class="sxs-lookup"><span data-stu-id="699be-153">String</span></span>|<span data-ttu-id="699be-154">`sectionGroups`ナビゲーションプロパティの URL。これは、ノートブック内のすべてのセクショングループを返します。</span><span class="sxs-lookup"><span data-stu-id="699be-154">The URL for the `sectionGroups` navigation property, which returns all the section groups in the notebook.</span></span> <span data-ttu-id="699be-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-155">Read-only.</span></span>|
|<span data-ttu-id="699be-156">sectionsUrl</span><span class="sxs-lookup"><span data-stu-id="699be-156">sectionsUrl</span></span>|<span data-ttu-id="699be-157">String</span><span class="sxs-lookup"><span data-stu-id="699be-157">String</span></span>|<span data-ttu-id="699be-158">ノートブック内のすべて`sections`のセクションを返すナビゲーションプロパティの URL。</span><span class="sxs-lookup"><span data-stu-id="699be-158">The URL for the `sections` navigation property, which returns all the sections in the notebook.</span></span> <span data-ttu-id="699be-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-159">Read-only.</span></span>|
|<span data-ttu-id="699be-160">self</span><span class="sxs-lookup"><span data-stu-id="699be-160">self</span></span>|<span data-ttu-id="699be-161">String</span><span class="sxs-lookup"><span data-stu-id="699be-161">String</span></span>|<span data-ttu-id="699be-162">ノートブックに関する詳細を取得できるエンドポイント。</span><span class="sxs-lookup"><span data-stu-id="699be-162">The endpoint where you can get details about the notebook.</span></span> <span data-ttu-id="699be-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-163">Read-only.</span></span>|
|<span data-ttu-id="699be-164">userRole</span><span class="sxs-lookup"><span data-stu-id="699be-164">userRole</span></span>|<span data-ttu-id="699be-165">String</span><span class="sxs-lookup"><span data-stu-id="699be-165">String</span></span>|<span data-ttu-id="699be-166">使用可能な値: `Owner`、`Contributor`、`Reader`、`None`。</span><span class="sxs-lookup"><span data-stu-id="699be-166">Possible values are: `Owner`, `Contributor`, `Reader`, `None`.</span></span> <span data-ttu-id="699be-167">Owner ノートブックへの所有者レベルのアクセス権を表します。</span><span class="sxs-lookup"><span data-stu-id="699be-167">Owner represents owner-level access to the notebook.</span></span> <span data-ttu-id="699be-168">共同作成者は、ノートブックへの読み取り/書き込みアクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="699be-168">Contributor represents read/write access to the notebook.</span></span> <span data-ttu-id="699be-169">閲覧者は、ノートブックへの読み取り専用アクセスを表します。</span><span class="sxs-lookup"><span data-stu-id="699be-169">Reader represents read-only access to the notebook.</span></span> <span data-ttu-id="699be-170">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="699be-170">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="699be-171">関係</span><span class="sxs-lookup"><span data-stu-id="699be-171">Relationships</span></span>
| <span data-ttu-id="699be-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="699be-172">Relationship</span></span> | <span data-ttu-id="699be-173">型</span><span class="sxs-lookup"><span data-stu-id="699be-173">Type</span></span>   |<span data-ttu-id="699be-174">説明</span><span class="sxs-lookup"><span data-stu-id="699be-174">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="699be-175">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="699be-175">sectionGroups</span></span>|<span data-ttu-id="699be-176">[sectionGroup](sectiongroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="699be-176">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="699be-177">ノートブック内のセクション グループ。</span><span class="sxs-lookup"><span data-stu-id="699be-177">The section groups in the notebook.</span></span> <span data-ttu-id="699be-178">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-178">Read-only.</span></span> <span data-ttu-id="699be-179">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="699be-179">Nullable.</span></span>|
|<span data-ttu-id="699be-180">セクション</span><span class="sxs-lookup"><span data-stu-id="699be-180">sections</span></span>|<span data-ttu-id="699be-181">[onenoteSection](onenotesection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="699be-181">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="699be-182">ノートブックのセクション。</span><span class="sxs-lookup"><span data-stu-id="699be-182">The sections in the notebook.</span></span> <span data-ttu-id="699be-183">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="699be-183">Read-only.</span></span> <span data-ttu-id="699be-184">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="699be-184">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="699be-185">メソッド</span><span class="sxs-lookup"><span data-stu-id="699be-185">Methods</span></span>

| <span data-ttu-id="699be-186">メソッド</span><span class="sxs-lookup"><span data-stu-id="699be-186">Method</span></span>           | <span data-ttu-id="699be-187">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="699be-187">Return Type</span></span>    |<span data-ttu-id="699be-188">説明</span><span class="sxs-lookup"><span data-stu-id="699be-188">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="699be-189">ノートブックを取得する</span><span class="sxs-lookup"><span data-stu-id="699be-189">Get notebook</span></span>](../api/notebook-get.md) | [<span data-ttu-id="699be-190">ノートブック</span><span class="sxs-lookup"><span data-stu-id="699be-190">notebook</span></span>](notebook.md) |<span data-ttu-id="699be-191">ノートブックのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="699be-191">Read the properties and relationships of the notebook.</span></span>|
|[<span data-ttu-id="699be-192">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="699be-192">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="699be-193">[recentNotebook](recentnotebook.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="699be-193">[recentNotebook](recentnotebook.md) collection</span></span> | <span data-ttu-id="699be-194">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="699be-194">Get a collection of the most recently accessed notebooks for the user.</span></span> |
|[<span data-ttu-id="699be-195">getNotebookFromWebUrl</span><span class="sxs-lookup"><span data-stu-id="699be-195">getNotebookFromWebUrl</span></span>](../api/notebook-getnotebookfromweburl.md) | [<span data-ttu-id="699be-196">ノートブック</span><span class="sxs-lookup"><span data-stu-id="699be-196">notebook</span></span>](notebook.md) | <span data-ttu-id="699be-197">URL パスを使用して、ノートブックオブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="699be-197">Retrieve the properties and relationships of a notebook object using its URL path.</span></span> |
|[<span data-ttu-id="699be-198">セクション グループを作成する</span><span class="sxs-lookup"><span data-stu-id="699be-198">Create section group</span></span>](../api/notebook-post-sectiongroups.md) |[<span data-ttu-id="699be-199">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="699be-199">sectionGroup</span></span>](sectiongroup.md)| <span data-ttu-id="699be-200">指定したノートブックの sectionGroups コレクションに投稿して、セクショングループを作成します。</span><span class="sxs-lookup"><span data-stu-id="699be-200">Create a section group by posting to the sectionGroups collection in the specified notebook.</span></span>|
|[<span data-ttu-id="699be-201">List section groups</span><span class="sxs-lookup"><span data-stu-id="699be-201">List section groups</span></span>](../api/notebook-list-sectiongroups.md) |<span data-ttu-id="699be-202">[sectionGroup](sectiongroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="699be-202">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="699be-203">指定されたノートブック内のセクショングループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="699be-203">Get a collection of section groups in the specified notebook.</span></span>|
|[<span data-ttu-id="699be-204">セクションを作成する</span><span class="sxs-lookup"><span data-stu-id="699be-204">Create section</span></span>](../api/notebook-post-sections.md) |[<span data-ttu-id="699be-205">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="699be-205">onenoteSection</span></span>](onenotesection.md)| <span data-ttu-id="699be-206">指定したノートブックの sections コレクションに投稿してセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="699be-206">Create a section by posting to the sections collection in the specified notebook.</span></span>|
|[<span data-ttu-id="699be-207">List sections</span><span class="sxs-lookup"><span data-stu-id="699be-207">List sections</span></span>](../api/notebook-list-sections.md) |<span data-ttu-id="699be-208">[onenoteSection](onenotesection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="699be-208">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="699be-209">指定されたノートブック内のセクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="699be-209">Get a collection of sections in the specified notebook.</span></span>|
|[<span data-ttu-id="699be-210">copyNotebook</span><span class="sxs-lookup"><span data-stu-id="699be-210">copyNotebook</span></span>](../api/notebook-copynotebook.md)| <span data-ttu-id="699be-211">None</span><span class="sxs-lookup"><span data-stu-id="699be-211">None</span></span> | <span data-ttu-id="699be-212">ノートブックをコピーします。</span><span class="sxs-lookup"><span data-stu-id="699be-212">Copies a notebook.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
