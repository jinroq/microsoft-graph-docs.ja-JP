---
title: section リソースの種類
description: OneNote ノートブックのセクションです。セクションには、ページを含めることができます。
localization_priority: Normal
ms.openlocfilehash: 181fa3399f13d0490d9cd7d4599d8208633107b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831857"
---
# <a name="section-resource-type"></a><span data-ttu-id="c7c44-104">section リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c7c44-104">section resource type</span></span>

> <span data-ttu-id="c7c44-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c7c44-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7c44-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c44-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7c44-p103">OneNote ノートブックのセクションです。セクションには、ページを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p103">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7c44-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c7c44-109">JSON representation</span></span>

<span data-ttu-id="c7c44-110">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="c7c44-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7c44-111">Properties</span></span>
| <span data-ttu-id="c7c44-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7c44-112">Property</span></span>     | <span data-ttu-id="c7c44-113">種類</span><span class="sxs-lookup"><span data-stu-id="c7c44-113">Type</span></span>   |<span data-ttu-id="c7c44-114">説明</span><span class="sxs-lookup"><span data-stu-id="c7c44-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7c44-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="c7c44-115">createdBy</span></span>|[<span data-ttu-id="c7c44-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="c7c44-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="c7c44-p104">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c7c44-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c44-119">createdDateTime</span></span>|<span data-ttu-id="c7c44-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c44-120">DateTimeOffset</span></span>|<span data-ttu-id="c7c44-p105">セクションが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p105">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="c7c44-125">id</span><span class="sxs-lookup"><span data-stu-id="c7c44-125">id</span></span>|<span data-ttu-id="c7c44-126">String</span><span class="sxs-lookup"><span data-stu-id="c7c44-126">String</span></span>|<span data-ttu-id="c7c44-p106">セクションの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p106">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="c7c44-129">isDefault</span><span class="sxs-lookup"><span data-stu-id="c7c44-129">isDefault</span></span>|<span data-ttu-id="c7c44-130">ブール型</span><span class="sxs-lookup"><span data-stu-id="c7c44-130">Boolean</span></span>|<span data-ttu-id="c7c44-p107">これがユーザーの既定のセクションであるかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p107">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="c7c44-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c7c44-133">lastModifiedBy</span></span>|[<span data-ttu-id="c7c44-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="c7c44-134">identitySet</span></span>](identityset.md)|<span data-ttu-id="c7c44-p108">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p108">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="c7c44-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c44-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c7c44-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c44-138">DateTimeOffset</span></span>|<span data-ttu-id="c7c44-p109">セクションが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p109">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="c7c44-143">links</span><span class="sxs-lookup"><span data-stu-id="c7c44-143">links</span></span>|[<span data-ttu-id="c7c44-144">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="c7c44-144">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="c7c44-p110">セクションを開くためのリンク。`oneNoteClientURL` リンクが OneNote のネイティブ クライアントでセクションを開きます (インストールされている場合)。`oneNoteWebURL` リンクでは、OneNote Online でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p110">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="c7c44-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c7c44-148">displayName</span></span>|<span data-ttu-id="c7c44-149">String</span><span class="sxs-lookup"><span data-stu-id="c7c44-149">String</span></span>|<span data-ttu-id="c7c44-150">セクションの名前。</span><span class="sxs-lookup"><span data-stu-id="c7c44-150">The name of the section.</span></span> |
|<span data-ttu-id="c7c44-151">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="c7c44-151">pagesUrl</span></span>|<span data-ttu-id="c7c44-152">String</span><span class="sxs-lookup"><span data-stu-id="c7c44-152">String</span></span>|<span data-ttu-id="c7c44-p111">セクション内のすべてのページに関する詳細情報を入手できる `pages` エンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p111">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="c7c44-155">self</span><span class="sxs-lookup"><span data-stu-id="c7c44-155">self</span></span>|<span data-ttu-id="c7c44-156">String</span><span class="sxs-lookup"><span data-stu-id="c7c44-156">String</span></span>|<span data-ttu-id="c7c44-p112">セクションに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p112">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7c44-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7c44-159">Relationships</span></span>
| <span data-ttu-id="c7c44-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c7c44-160">Relationship</span></span> | <span data-ttu-id="c7c44-161">型</span><span class="sxs-lookup"><span data-stu-id="c7c44-161">Type</span></span>   |<span data-ttu-id="c7c44-162">説明</span><span class="sxs-lookup"><span data-stu-id="c7c44-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7c44-163">pages</span><span class="sxs-lookup"><span data-stu-id="c7c44-163">pages</span></span>|<span data-ttu-id="c7c44-164">[Page](page.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c7c44-164">[Page](page.md) collection</span></span>|<span data-ttu-id="c7c44-p113">セクション内のページのコレクションです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p113">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="c7c44-168">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="c7c44-168">parentNotebook</span></span>|[<span data-ttu-id="c7c44-169">Notebook</span><span class="sxs-lookup"><span data-stu-id="c7c44-169">Notebook</span></span>](notebook.md)|<span data-ttu-id="c7c44-p114">セクションを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p114">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="c7c44-172">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="c7c44-172">parentSectionGroup</span></span>|[<span data-ttu-id="c7c44-173">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="c7c44-173">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="c7c44-p115">セクションを含むセクション グループ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c7c44-p115">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="c7c44-176">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7c44-176">Methods</span></span>

| <span data-ttu-id="c7c44-177">メソッド</span><span class="sxs-lookup"><span data-stu-id="c7c44-177">Method</span></span>           | <span data-ttu-id="c7c44-178">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c7c44-178">Return Type</span></span>    |<span data-ttu-id="c7c44-179">説明</span><span class="sxs-lookup"><span data-stu-id="c7c44-179">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7c44-180">Get section</span><span class="sxs-lookup"><span data-stu-id="c7c44-180">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="c7c44-181">Section</span><span class="sxs-lookup"><span data-stu-id="c7c44-181">Section</span></span>](section.md) |<span data-ttu-id="c7c44-182">セクションのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c7c44-182">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="c7c44-183">Create page</span><span class="sxs-lookup"><span data-stu-id="c7c44-183">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="c7c44-184">Page</span><span class="sxs-lookup"><span data-stu-id="c7c44-184">Page</span></span>](page.md)| <span data-ttu-id="c7c44-185">指定されたセクションでページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="c7c44-185">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="c7c44-186">List pages</span><span class="sxs-lookup"><span data-stu-id="c7c44-186">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="c7c44-187">[Page](page.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c7c44-187">[Page](page.md) collection</span></span>| <span data-ttu-id="c7c44-188">指定されたセクション内のページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="c7c44-188">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="c7c44-189">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="c7c44-189">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="c7c44-190">なし</span><span class="sxs-lookup"><span data-stu-id="c7c44-190">None</span></span>|<span data-ttu-id="c7c44-191">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="c7c44-191">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="c7c44-192">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="c7c44-192">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="c7c44-193">なし</span><span class="sxs-lookup"><span data-stu-id="c7c44-193">None</span></span>|<span data-ttu-id="c7c44-194">特定のセクション グループにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="c7c44-194">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
