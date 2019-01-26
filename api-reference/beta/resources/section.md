---
title: section リソースの種類
description: OneNote ノートブックのセクションです。セクションには、ページを含めることができます。
localization_priority: Normal
ms.openlocfilehash: ea33cfae128a7ea796f3f14bd165210cbfec121d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574139"
---
# <a name="section-resource-type"></a><span data-ttu-id="73505-104">section リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73505-104">section resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73505-p102">OneNote ノートブックのセクションです。セクションには、ページを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="73505-p102">A section in a OneNote notebook. Sections can contain pages.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73505-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="73505-107">JSON representation</span></span>

<span data-ttu-id="73505-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="73505-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="73505-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73505-109">Properties</span></span>
| <span data-ttu-id="73505-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73505-110">Property</span></span>     | <span data-ttu-id="73505-111">型</span><span class="sxs-lookup"><span data-stu-id="73505-111">Type</span></span>   |<span data-ttu-id="73505-112">説明</span><span class="sxs-lookup"><span data-stu-id="73505-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73505-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="73505-113">createdBy</span></span>|[<span data-ttu-id="73505-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="73505-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="73505-p103">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="73505-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73505-117">createdDateTime</span></span>|<span data-ttu-id="73505-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73505-118">DateTimeOffset</span></span>|<span data-ttu-id="73505-p104">セクションが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p104">The date and time when the section was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="73505-123">id</span><span class="sxs-lookup"><span data-stu-id="73505-123">id</span></span>|<span data-ttu-id="73505-124">String</span><span class="sxs-lookup"><span data-stu-id="73505-124">String</span></span>|<span data-ttu-id="73505-p105">セクションの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p105">The unique identifier of the section.  Read-only.</span></span>|
|<span data-ttu-id="73505-127">isDefault</span><span class="sxs-lookup"><span data-stu-id="73505-127">isDefault</span></span>|<span data-ttu-id="73505-128">ブール値</span><span class="sxs-lookup"><span data-stu-id="73505-128">Boolean</span></span>|<span data-ttu-id="73505-p106">これがユーザーの既定のセクションであるかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p106">Indicates whether this is the user's default section. Read-only.</span></span>|
|<span data-ttu-id="73505-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="73505-131">lastModifiedBy</span></span>|[<span data-ttu-id="73505-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="73505-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="73505-p107">そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p107">Identity of the user, device, and application which created the item. Read-only.</span></span>|
|<span data-ttu-id="73505-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73505-135">lastModifiedDateTime</span></span>|<span data-ttu-id="73505-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73505-136">DateTimeOffset</span></span>|<span data-ttu-id="73505-p108">セクションが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p108">The date and time when the section was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="73505-141">links</span><span class="sxs-lookup"><span data-stu-id="73505-141">links</span></span>|[<span data-ttu-id="73505-142">sectionLinks</span><span class="sxs-lookup"><span data-stu-id="73505-142">sectionLinks</span></span>](sectionlinks.md)|<span data-ttu-id="73505-p109">セクションを開くためのリンク。`oneNoteClientURL` リンクが OneNote のネイティブ クライアントでセクションを開きます (インストールされている場合)。`oneNoteWebURL` リンクでは、OneNote Online でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="73505-p109">Links for opening the section. The `oneNoteClientURL` link opens the section in the OneNote native client if it's installed. The `oneNoteWebURL` link opens the section in OneNote Online.</span></span>|
|<span data-ttu-id="73505-146">displayName</span><span class="sxs-lookup"><span data-stu-id="73505-146">displayName</span></span>|<span data-ttu-id="73505-147">String</span><span class="sxs-lookup"><span data-stu-id="73505-147">String</span></span>|<span data-ttu-id="73505-148">セクションの名前。</span><span class="sxs-lookup"><span data-stu-id="73505-148">The name of the section.</span></span> |
|<span data-ttu-id="73505-149">pagesUrl</span><span class="sxs-lookup"><span data-stu-id="73505-149">pagesUrl</span></span>|<span data-ttu-id="73505-150">String</span><span class="sxs-lookup"><span data-stu-id="73505-150">String</span></span>|<span data-ttu-id="73505-p110">セクション内のすべてのページに関する詳細情報を入手できる `pages` エンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p110">The `pages` endpoint where you can get details for all the pages in the section. Read-only.</span></span>|
|<span data-ttu-id="73505-153">self</span><span class="sxs-lookup"><span data-stu-id="73505-153">self</span></span>|<span data-ttu-id="73505-154">String</span><span class="sxs-lookup"><span data-stu-id="73505-154">String</span></span>|<span data-ttu-id="73505-p111">セクションに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p111">The endpoint where you can get details about the section. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73505-157">関係</span><span class="sxs-lookup"><span data-stu-id="73505-157">Relationships</span></span>
| <span data-ttu-id="73505-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="73505-158">Relationship</span></span> | <span data-ttu-id="73505-159">型</span><span class="sxs-lookup"><span data-stu-id="73505-159">Type</span></span>   |<span data-ttu-id="73505-160">説明</span><span class="sxs-lookup"><span data-stu-id="73505-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73505-161">pages</span><span class="sxs-lookup"><span data-stu-id="73505-161">pages</span></span>|<span data-ttu-id="73505-162">[onenotePage](onenotepage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="73505-162">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="73505-p112">セクション内のページのコレクションです。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="73505-p112">The collection of pages in the section.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="73505-166">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="73505-166">parentNotebook</span></span>|[<span data-ttu-id="73505-167">ノートブック</span><span class="sxs-lookup"><span data-stu-id="73505-167">notebook</span></span>](notebook.md)|<span data-ttu-id="73505-p113">セクションを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p113">The notebook that contains the section.  Read-only.</span></span>|
|<span data-ttu-id="73505-170">parentSectionGroup</span><span class="sxs-lookup"><span data-stu-id="73505-170">parentSectionGroup</span></span>|[<span data-ttu-id="73505-171">sectionGroup</span><span class="sxs-lookup"><span data-stu-id="73505-171">sectionGroup</span></span>](sectiongroup.md)|<span data-ttu-id="73505-p114">セクションを含むセクション グループ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="73505-p114">The section group that contains the section.  Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="73505-174">メソッド</span><span class="sxs-lookup"><span data-stu-id="73505-174">Methods</span></span>

| <span data-ttu-id="73505-175">メソッド</span><span class="sxs-lookup"><span data-stu-id="73505-175">Method</span></span>           | <span data-ttu-id="73505-176">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="73505-176">Return Type</span></span>    |<span data-ttu-id="73505-177">説明</span><span class="sxs-lookup"><span data-stu-id="73505-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73505-178">Get section</span><span class="sxs-lookup"><span data-stu-id="73505-178">Get section</span></span>](../api/section-get.md) | [<span data-ttu-id="73505-179">onenoteSection</span><span class="sxs-lookup"><span data-stu-id="73505-179">onenoteSection</span></span>](section.md) |<span data-ttu-id="73505-180">セクションのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="73505-180">Read the properties and relationships of the section.</span></span>|
|[<span data-ttu-id="73505-181">Create page</span><span class="sxs-lookup"><span data-stu-id="73505-181">Create page</span></span>](../api/section-post-pages.md) |[<span data-ttu-id="73505-182">onenotePage</span><span class="sxs-lookup"><span data-stu-id="73505-182">onenotePage</span></span>](onenotepage.md)| <span data-ttu-id="73505-183">指定されたセクションでページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="73505-183">Create a page by posting to the pages collection in the specified section.</span></span>|
|[<span data-ttu-id="73505-184">List pages</span><span class="sxs-lookup"><span data-stu-id="73505-184">List pages</span></span>](../api/section-list-pages.md) |<span data-ttu-id="73505-185">[onenotePage](onenotepage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="73505-185">[onenotePage](onenotepage.md) collection</span></span>| <span data-ttu-id="73505-186">指定されたセクション内のページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="73505-186">Get a collection of pages in the specified section.</span></span>|
|[<span data-ttu-id="73505-187">copyToNotebook</span><span class="sxs-lookup"><span data-stu-id="73505-187">copyToNotebook</span></span>](../api/section-copytonotebook.md)|<span data-ttu-id="73505-188">なし</span><span class="sxs-lookup"><span data-stu-id="73505-188">None</span></span>|<span data-ttu-id="73505-189">特定のノートブックにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="73505-189">Copy the section to a specific notebook.</span></span>|
|[<span data-ttu-id="73505-190">copyToSectionGroup</span><span class="sxs-lookup"><span data-stu-id="73505-190">copyToSectionGroup</span></span>](../api/section-copytosectiongroup.md)|<span data-ttu-id="73505-191">なし</span><span class="sxs-lookup"><span data-stu-id="73505-191">None</span></span>|<span data-ttu-id="73505-192">特定のセクション グループにセクションをコピーします。</span><span class="sxs-lookup"><span data-stu-id="73505-192">Copy the section to a specific section group.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteSection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/section.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
