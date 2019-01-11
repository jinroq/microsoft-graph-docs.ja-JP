---
title: section リソースの種類
description: OneNote ノートブックのセクションです。セクションには、ページを含めることができます。
localization_priority: Normal
ms.openlocfilehash: f9cb5a8e3ddf9cf4a045103e4ecc7909653d797c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853236"
---
# <a name="section-resource-type"></a><span data-ttu-id="f026b-104">section リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f026b-104">section resource type</span></span>

<span data-ttu-id="f026b-p102">OneNote ノートブックのセクションです。セクションには、ページを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f026b-p102">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f026b-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f026b-107">JSON representation</span></span>

<span data-ttu-id="f026b-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f026b-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f026b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f026b-109">Properties</span></span>
| <span data-ttu-id="f026b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f026b-110">Property</span></span>     | <span data-ttu-id="f026b-111">種類</span><span class="sxs-lookup"><span data-stu-id="f026b-111">Type</span></span>   |<span data-ttu-id="f026b-112">説明</span><span class="sxs-lookup"><span data-stu-id="f026b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f026b-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="f026b-113">createdBy</span></span>|[<span data-ttu-id="f026b-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="f026b-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="f026b-p103">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="f026b-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f026b-117">createdDateTime</span></span>|<span data-ttu-id="f026b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f026b-118">DateTimeOffset</span></span>|<span data-ttu-id="f026b-p104">セクションが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p104">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="f026b-123">id</span><span class="sxs-lookup"><span data-stu-id="f026b-123">id</span></span>|<span data-ttu-id="f026b-124">String</span><span class="sxs-lookup"><span data-stu-id="f026b-124">String</span></span>|<span data-ttu-id="f026b-p105">セクションの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p105">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="f026b-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="f026b-127">isDefault</span></span>|<span data-ttu-id="f026b-128">ブール型</span><span class="sxs-lookup"><span data-stu-id="f026b-128">Boolean</span></span>|<span data-ttu-id="f026b-p106">これがユーザーの既定のセクションであるかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p106">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="f026b-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f026b-131">lastModifiedBy</span></span>|[<span data-ttu-id="f026b-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="f026b-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="f026b-p107">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="f026b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f026b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f026b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f026b-136">DateTimeOffset</span></span>|<span data-ttu-id="f026b-p108">セクションが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p108">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="f026b-141">links</span><span class="sxs-lookup"><span data-stu-id="f026b-141">links</span></span>|[<span data-ttu-id="f026b-142">SectionLinks</span><span class="sxs-lookup"><span data-stu-id="f026b-142">SectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="f026b-p109">セクションを開くためのリンク。`oneNoteClientURL` リンクが OneNote のネイティブ クライアントでセクションを開きます (インストールされている場合)。`oneNoteWebURL` リンクでは、OneNote Online でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="f026b-p109">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="f026b-146">displayName</span><span class="sxs-lookup"><span data-stu-id="f026b-146">displayName</span></span>|<span data-ttu-id="f026b-147">String</span><span class="sxs-lookup"><span data-stu-id="f026b-147">String</span></span>|<span data-ttu-id="f026b-148">セクションの名前。</span><span class="sxs-lookup"><span data-stu-id="f026b-148">The name of the section.</span></span> |
|<span data-ttu-id="f026b-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="f026b-149">pagesUrl</span></span>|<span data-ttu-id="f026b-150">String</span><span class="sxs-lookup"><span data-stu-id="f026b-150">String</span></span>|<span data-ttu-id="f026b-p110">セクション内のすべてのページに関する詳細情報を入手できる `pages` エンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p110">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="f026b-153">self</span><span class="sxs-lookup"><span data-stu-id="f026b-153">self</span></span>|<span data-ttu-id="f026b-154">String</span><span class="sxs-lookup"><span data-stu-id="f026b-154">String</span></span>|<span data-ttu-id="f026b-p111">セクションに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p111">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f026b-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f026b-157">Relationships</span></span>
| <span data-ttu-id="f026b-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f026b-158">Relationship</span></span> | <span data-ttu-id="f026b-159">型</span><span class="sxs-lookup"><span data-stu-id="f026b-159">Type</span></span>   |<span data-ttu-id="f026b-160">説明</span><span class="sxs-lookup"><span data-stu-id="f026b-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f026b-161">pages</span><span class="sxs-lookup"><span data-stu-id="f026b-161">pages</span></span>|<span data-ttu-id="f026b-162">[OnenotePage](page.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f026b-162">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="f026b-p112">セクション内のページのコレクションです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f026b-p112">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="f026b-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="f026b-166">parentNotebook</span></span>|[<span data-ttu-id="f026b-167">Notebook</span><span class="sxs-lookup"><span data-stu-id="f026b-167">Notebook</span></span>](notebook.md)|<span data-ttu-id="f026b-p113">セクションを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p113">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="f026b-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="f026b-170">parentSectionGroup</span></span>|[<span data-ttu-id="f026b-171">SectionGroup</span><span class="sxs-lookup"><span data-stu-id="f026b-171">SectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="f026b-p114">セクションを含むセクション グループ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f026b-p114">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="f026b-174">メソッド</span><span class="sxs-lookup"><span data-stu-id="f026b-174">Methods</span></span>

| <span data-ttu-id="f026b-175">メソッド</span><span class="sxs-lookup"><span data-stu-id="f026b-175">Method</span></span>           | <span data-ttu-id="f026b-176">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f026b-176">Return Type</span></span>    |<span data-ttu-id="f026b-177">説明</span><span class="sxs-lookup"><span data-stu-id="f026b-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f026b-178">Get section</span><span class="sxs-lookup"><span data-stu-id="f026b-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="f026b-179">OnenoteSection</span><span class="sxs-lookup"><span data-stu-id="f026b-179">OnenoteSection</span></span>](section.md) |<span data-ttu-id="f026b-180">セクションのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f026b-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="f026b-181">Create page</span><span class="sxs-lookup"><span data-stu-id="f026b-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="f026b-182">Page</span><span class="sxs-lookup"><span data-stu-id="f026b-182">Page</span></span>](page.md)| <span data-ttu-id="f026b-183">指定されたセクションでページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="f026b-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="f026b-184">List pages</span><span class="sxs-lookup"><span data-stu-id="f026b-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="f026b-185">[Page](page.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f026b-185">[Page](page.md) collection</span></span>| <span data-ttu-id="f026b-186">指定されたセクション内のページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f026b-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="f026b-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="f026b-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="f026b-188">なし</span><span class="sxs-lookup"><span data-stu-id="f026b-188">None</span></span>|<span data-ttu-id="f026b-189">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="f026b-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="f026b-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="f026b-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="f026b-191">なし</span><span class="sxs-lookup"><span data-stu-id="f026b-191">None</span></span>|<span data-ttu-id="f026b-192">特定のセクション グループにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="f026b-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
