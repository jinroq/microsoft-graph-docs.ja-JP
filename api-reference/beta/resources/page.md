---
title: page リソースの種類
description: OneNote ノートブックのページです。
ms.openlocfilehash: 82b9ca00cb4488c33e73daa94844b11f8de301cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071986"
---
# <a name="page-resource-type"></a><span data-ttu-id="39ccc-103">page リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39ccc-103">page resource type</span></span>

> <span data-ttu-id="39ccc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="39ccc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39ccc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39ccc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39ccc-106">OneNote ノートブックのページです。</span><span class="sxs-lookup"><span data-stu-id="39ccc-106">A page in a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39ccc-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39ccc-107">JSON representation</span></span>

<span data-ttu-id="39ccc-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="39ccc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39ccc-109">Properties</span></span>
| <span data-ttu-id="39ccc-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39ccc-110">Property</span></span>     | <span data-ttu-id="39ccc-111">型</span><span class="sxs-lookup"><span data-stu-id="39ccc-111">Type</span></span>   |<span data-ttu-id="39ccc-112">説明</span><span class="sxs-lookup"><span data-stu-id="39ccc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39ccc-113">content</span><span class="sxs-lookup"><span data-stu-id="39ccc-113">content</span></span>|<span data-ttu-id="39ccc-114">Stream</span><span class="sxs-lookup"><span data-stu-id="39ccc-114">Stream</span></span>|<span data-ttu-id="39ccc-115">ページの HTML コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="39ccc-115">The page's HTML content.</span></span>|
|<span data-ttu-id="39ccc-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="39ccc-116">contentUrl</span></span>|<span data-ttu-id="39ccc-117">String</span><span class="sxs-lookup"><span data-stu-id="39ccc-117">String</span></span>|<span data-ttu-id="39ccc-p102">ページの HTML コンテンツの URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p102">The URL for the page's HTML content.  Read-only.</span></span>|
|<span data-ttu-id="39ccc-120">createdByAppId</span><span class="sxs-lookup"><span data-stu-id="39ccc-120">createdByAppId</span></span>|<span data-ttu-id="39ccc-121">String</span><span class="sxs-lookup"><span data-stu-id="39ccc-121">String</span></span>|<span data-ttu-id="39ccc-p103">ページを作成したアプリケーションの一意の識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p103">The unique identifier of the application that created the page. Read-only.</span></span>|
|<span data-ttu-id="39ccc-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39ccc-124">createdDateTime</span></span>|<span data-ttu-id="39ccc-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ccc-125">DateTimeOffset</span></span>|<span data-ttu-id="39ccc-p104">ページが作成された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p104">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="39ccc-130">id</span><span class="sxs-lookup"><span data-stu-id="39ccc-130">id</span></span>|<span data-ttu-id="39ccc-131">String</span><span class="sxs-lookup"><span data-stu-id="39ccc-131">String</span></span>|<span data-ttu-id="39ccc-p105">ページの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p105">The unique identifier of the page.  Read-only.</span></span>|
|<span data-ttu-id="39ccc-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ccc-134">lastModifiedDateTime</span></span>|<span data-ttu-id="39ccc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ccc-135">DateTimeOffset</span></span>|<span data-ttu-id="39ccc-p106">ページが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p106">The date and time when the page was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="39ccc-140">level</span><span class="sxs-lookup"><span data-stu-id="39ccc-140">level</span></span>|<span data-ttu-id="39ccc-141">Int32</span><span class="sxs-lookup"><span data-stu-id="39ccc-141">Int32</span></span>|<span data-ttu-id="39ccc-p107">ページのインデント レベル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p107">The indentation level of the page. Read-only.</span></span>|
|<span data-ttu-id="39ccc-144">links</span><span class="sxs-lookup"><span data-stu-id="39ccc-144">links</span></span>|[<span data-ttu-id="39ccc-145">PageLinks</span><span class="sxs-lookup"><span data-stu-id="39ccc-145">PageLinks</span></span>](pagelinks.md)|<span data-ttu-id="39ccc-p108">ページを開くためのリンク。`oneNoteClientURL`リンクが OneNote のネイティブ クライアントでページを開きます (インストールされている場合)。`oneNoteWebUrl` リンクでは、OneNote オンラインでページを開きます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p108">Links for opening the page. The `oneNoteClientURL` link opens the page in the OneNote native client if it 's installed. The `oneNoteWebUrl` link opens the page in OneNote Online. Read-only.</span></span>|
|<span data-ttu-id="39ccc-150">order</span><span class="sxs-lookup"><span data-stu-id="39ccc-150">order</span></span>|<span data-ttu-id="39ccc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="39ccc-151">Int32</span></span>|<span data-ttu-id="39ccc-p109">親セクション内でのページの順序。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p109">The order of the page within its parent section. Read-only.</span></span>|
|<span data-ttu-id="39ccc-154">self</span><span class="sxs-lookup"><span data-stu-id="39ccc-154">self</span></span>|<span data-ttu-id="39ccc-155">String</span><span class="sxs-lookup"><span data-stu-id="39ccc-155">String</span></span>|<span data-ttu-id="39ccc-p110">ページに関する詳細情報を入手できるエンドポイント。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p110">The endpoint where you can get details about the page. Read-only.</span></span>|
|<span data-ttu-id="39ccc-158">タイトル</span><span class="sxs-lookup"><span data-stu-id="39ccc-158">title</span></span>|<span data-ttu-id="39ccc-159">String</span><span class="sxs-lookup"><span data-stu-id="39ccc-159">String</span></span>|<span data-ttu-id="39ccc-160">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="39ccc-160">The title of the page.</span></span> |

## <a name="relationships"></a><span data-ttu-id="39ccc-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39ccc-161">Relationships</span></span>
| <span data-ttu-id="39ccc-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39ccc-162">Relationship</span></span> | <span data-ttu-id="39ccc-163">型</span><span class="sxs-lookup"><span data-stu-id="39ccc-163">Type</span></span>   |<span data-ttu-id="39ccc-164">説明</span><span class="sxs-lookup"><span data-stu-id="39ccc-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39ccc-165">parentNotebook</span><span class="sxs-lookup"><span data-stu-id="39ccc-165">parentNotebook</span></span>|[<span data-ttu-id="39ccc-166">Notebook</span><span class="sxs-lookup"><span data-stu-id="39ccc-166">Notebook</span></span>](notebook.md)|<span data-ttu-id="39ccc-p111">ページを含むノートブック。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p111">The notebook that contains the page.  Read-only.</span></span>|
|<span data-ttu-id="39ccc-169">parentSection</span><span class="sxs-lookup"><span data-stu-id="39ccc-169">parentSection</span></span>|[<span data-ttu-id="39ccc-170">Section</span><span class="sxs-lookup"><span data-stu-id="39ccc-170">Section</span></span>](section.md)|<span data-ttu-id="39ccc-p112">ページを含むセクション。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="39ccc-p112">The section that contains the page. Read-only.</span></span>|

## <a name="methods"></a><span data-ttu-id="39ccc-173">メソッド</span><span class="sxs-lookup"><span data-stu-id="39ccc-173">Methods</span></span>

| <span data-ttu-id="39ccc-174">メソッド</span><span class="sxs-lookup"><span data-stu-id="39ccc-174">Method</span></span>           | <span data-ttu-id="39ccc-175">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="39ccc-175">Return Type</span></span>    |<span data-ttu-id="39ccc-176">説明</span><span class="sxs-lookup"><span data-stu-id="39ccc-176">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="39ccc-177">Get page</span><span class="sxs-lookup"><span data-stu-id="39ccc-177">Get page</span></span>](../api/page-get.md) | [<span data-ttu-id="39ccc-178">Page</span><span class="sxs-lookup"><span data-stu-id="39ccc-178">Page</span></span>](page.md) |<span data-ttu-id="39ccc-179">ページのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="39ccc-179">Read the properties and relationships of the page.</span></span>|
|[<span data-ttu-id="39ccc-180">Update page content</span><span class="sxs-lookup"><span data-stu-id="39ccc-180">Update page content</span></span>](../api/page-update.md) | <span data-ttu-id="39ccc-181">なし</span><span class="sxs-lookup"><span data-stu-id="39ccc-181">None</span></span> |<span data-ttu-id="39ccc-182">ページの HTML コンテンツを更新します。</span><span class="sxs-lookup"><span data-stu-id="39ccc-182">Update the HTML content of the page.</span></span> |
|[<span data-ttu-id="39ccc-183">Delete page</span><span class="sxs-lookup"><span data-stu-id="39ccc-183">Delete page</span></span>](../api/page-delete.md) | <span data-ttu-id="39ccc-184">なし</span><span class="sxs-lookup"><span data-stu-id="39ccc-184">None</span></span> |<span data-ttu-id="39ccc-185">ページを削除します。</span><span class="sxs-lookup"><span data-stu-id="39ccc-185">Delete the page.</span></span> |
|[<span data-ttu-id="39ccc-186">copyToSection</span><span class="sxs-lookup"><span data-stu-id="39ccc-186">copyToSection</span></span>](../api/page-copytosection.md)| <span data-ttu-id="39ccc-187">なし</span><span class="sxs-lookup"><span data-stu-id="39ccc-187">None</span></span> |<span data-ttu-id="39ccc-188">特定のセクションにページをコピーします。</span><span class="sxs-lookup"><span data-stu-id="39ccc-188">Copies the page to a specific section.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->