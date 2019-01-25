---
title: page リソースの種類
description: OneNote ノートブックのページです。
localization_priority: Normal
ms.openlocfilehash: d8c27cdc144e9b192bd0205f256653ff7f04df5f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519242"
---
# <a name="page-resource-type"></a><span data-ttu-id="ef6dd-103">page リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef6dd-103">page resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef6dd-104">OneNote ノートブックのページです。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-104">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef6dd-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef6dd-105">JSON representation</span></span>

<span data-ttu-id="ef6dd-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "parentNotebook",
    "parentSection"
  ],
  "@odata.type": "microsoft.graph.onenotePage"
}-->

```json
{
  "content": "stream",
  "contentUrl": "string",
  "createdByAppId": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "level": 1024,
  "links": {"@odata.type": "microsoft.graph.pageLinks"},
  "order": 1024,
  "self": "string",
  "title": "string"
}

```
## <a name="properties"></a><span data-ttu-id="ef6dd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef6dd-107">Properties</span></span>
| <span data-ttu-id="ef6dd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef6dd-108">Property</span></span>     | <span data-ttu-id="ef6dd-109">型</span><span class="sxs-lookup"><span data-stu-id="ef6dd-109">Type</span></span>   |<span data-ttu-id="ef6dd-110">説明</span><span class="sxs-lookup"><span data-stu-id="ef6dd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef6dd-111">content</span><span class="sxs-lookup"><span data-stu-id="ef6dd-111">content</span></span>|<span data-ttu-id="ef6dd-112">Stream</span><span class="sxs-lookup"><span data-stu-id="ef6dd-112">Stream</span></span>|<span data-ttu-id="ef6dd-113">ページの HTML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-113">The page's HTML content.</span></span>|
|<span data-ttu-id="ef6dd-114">contentUrl</span><span class="sxs-lookup"><span data-stu-id="ef6dd-114">contentUrl</span></span>|<span data-ttu-id="ef6dd-115">String</span><span class="sxs-lookup"><span data-stu-id="ef6dd-115">String</span></span>|<span data-ttu-id="ef6dd-p101">ページの HTML コンテンツの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p101">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="ef6dd-118">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="ef6dd-118">createdByAppId</span></span>|<span data-ttu-id="ef6dd-119">String</span><span class="sxs-lookup"><span data-stu-id="ef6dd-119">String</span></span>|<span data-ttu-id="ef6dd-p102">ページを作成したアプリケーションの一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p102">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="ef6dd-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef6dd-122">createdDateTime</span></span>|<span data-ttu-id="ef6dd-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef6dd-123">DateTimeOffset</span></span>|<span data-ttu-id="ef6dd-p103">ページが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p103">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="ef6dd-128">id</span><span class="sxs-lookup"><span data-stu-id="ef6dd-128">id</span></span>|<span data-ttu-id="ef6dd-129">文字列</span><span class="sxs-lookup"><span data-stu-id="ef6dd-129">String</span></span>|<span data-ttu-id="ef6dd-p104">ページの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p104">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="ef6dd-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef6dd-132">lastModifiedDateTime</span></span>|<span data-ttu-id="ef6dd-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef6dd-133">DateTimeOffset</span></span>|<span data-ttu-id="ef6dd-p105">ページが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p105">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="ef6dd-138">level</span><span class="sxs-lookup"><span data-stu-id="ef6dd-138">level</span></span>|<span data-ttu-id="ef6dd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ef6dd-139">Int32</span></span>|<span data-ttu-id="ef6dd-p106">ページのインデント レベル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p106">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="ef6dd-142">links</span><span class="sxs-lookup"><span data-stu-id="ef6dd-142">links</span></span>|[<span data-ttu-id="ef6dd-143">PageLinks</span><span class="sxs-lookup"><span data-stu-id="ef6dd-143">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="ef6dd-p107">ページを開くためのリンク。`oneNoteClientURL`リンクが OneNote のネイティブ クライアントでページを開きます (インストールされている場合)。`oneNoteWebUrl` リンクでは、OneNote オンラインでページを開きます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p107">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="ef6dd-148">order</span><span class="sxs-lookup"><span data-stu-id="ef6dd-148">order</span></span>|<span data-ttu-id="ef6dd-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ef6dd-149">Int32</span></span>|<span data-ttu-id="ef6dd-p108">親セクション内でのページの順序。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p108">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="ef6dd-152">self</span><span class="sxs-lookup"><span data-stu-id="ef6dd-152">self</span></span>|<span data-ttu-id="ef6dd-153">String</span><span class="sxs-lookup"><span data-stu-id="ef6dd-153">String</span></span>|<span data-ttu-id="ef6dd-p109">ページに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p109">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="ef6dd-156">タイトル</span><span class="sxs-lookup"><span data-stu-id="ef6dd-156">title</span></span>|<span data-ttu-id="ef6dd-157">String</span><span class="sxs-lookup"><span data-stu-id="ef6dd-157">String</span></span>|<span data-ttu-id="ef6dd-158">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-158">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ef6dd-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef6dd-159">Relationships</span></span>
| <span data-ttu-id="ef6dd-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef6dd-160">Relationship</span></span> | <span data-ttu-id="ef6dd-161">型</span><span class="sxs-lookup"><span data-stu-id="ef6dd-161">Type</span></span>   |<span data-ttu-id="ef6dd-162">説明</span><span class="sxs-lookup"><span data-stu-id="ef6dd-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef6dd-163">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="ef6dd-163">parentNotebook</span></span>|[<span data-ttu-id="ef6dd-164">Notebook</span><span class="sxs-lookup"><span data-stu-id="ef6dd-164">Notebook</span></span>](notebook.md)|<span data-ttu-id="ef6dd-p110">ページを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p110">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="ef6dd-167">parentSection</span><span class="sxs-lookup"><span data-stu-id="ef6dd-167">parentSection</span></span>|[<span data-ttu-id="ef6dd-168">Section</span><span class="sxs-lookup"><span data-stu-id="ef6dd-168">Section</span></span>](section.md)|<span data-ttu-id="ef6dd-p111">ページを含むセクション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-p111">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="ef6dd-171">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef6dd-171">Methods</span></span>

| <span data-ttu-id="ef6dd-172">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef6dd-172">Method</span></span>           | <span data-ttu-id="ef6dd-173">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ef6dd-173">Return Type</span></span>    |<span data-ttu-id="ef6dd-174">説明</span><span class="sxs-lookup"><span data-stu-id="ef6dd-174">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef6dd-175">Get page</span><span class="sxs-lookup"><span data-stu-id="ef6dd-175">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="ef6dd-176">Page</span><span class="sxs-lookup"><span data-stu-id="ef6dd-176">Page</span></span>](page.md) |<span data-ttu-id="ef6dd-177">ページのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-177">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="ef6dd-178">Update page content</span><span class="sxs-lookup"><span data-stu-id="ef6dd-178">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="ef6dd-179">なし</span><span class="sxs-lookup"><span data-stu-id="ef6dd-179">None</span></span> |<span data-ttu-id="ef6dd-180">ページの HTML コンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-180">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="ef6dd-181">Delete page</span><span class="sxs-lookup"><span data-stu-id="ef6dd-181">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="ef6dd-182">なし</span><span class="sxs-lookup"><span data-stu-id="ef6dd-182">None</span></span> |<span data-ttu-id="ef6dd-183">ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-183">Delete the page.</span></span> |
|[<span data-ttu-id="ef6dd-184">copyToSection</span><span class="sxs-lookup"><span data-stu-id="ef6dd-184">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="ef6dd-185">なし</span><span class="sxs-lookup"><span data-stu-id="ef6dd-185">None</span></span> |<span data-ttu-id="ef6dd-186">特定のセクションにページをコピーします。</span><span class="sxs-lookup"><span data-stu-id="ef6dd-186">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/page.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
