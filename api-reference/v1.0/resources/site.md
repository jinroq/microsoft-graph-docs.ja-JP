---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
ms.openlocfilehash: db465f93f336a51d862daf6e05b1d6bc422247ea
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="site-resource"></a><span data-ttu-id="ad97e-102">Site リソース</span><span class="sxs-lookup"><span data-stu-id="ad97e-102">Site resource</span></span>

<span data-ttu-id="ad97e-103">**サイト** リソースは、メタデータと SharePoint サイトのリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="ad97e-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="ad97e-104">タスク</span><span class="sxs-lookup"><span data-stu-id="ad97e-104">Tasks</span></span>

<span data-ttu-id="ad97e-105">以下のすべての例は、`https://graph.microsoft.com/v1.0` からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="ad97e-106">タスク名</span><span class="sxs-lookup"><span data-stu-id="ad97e-106">Task name</span></span>                | <span data-ttu-id="ad97e-107">要求の例</span><span class="sxs-lookup"><span data-stu-id="ad97e-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="ad97e-108">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="ad97e-108">[Get root site][]</span></span>        | <span data-ttu-id="ad97e-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="ad97e-109">GET /sites/root</span></span>
| <span data-ttu-id="ad97e-110">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="ad97e-110">[Get site][]</span></span>             | <span data-ttu-id="ad97e-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="ad97e-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="ad97e-112">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="ad97e-112">[Get site by path][]</span></span>     | <span data-ttu-id="ad97e-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="ad97e-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="ad97e-114">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="ad97e-114">[Get site for a group][]</span></span> | <span data-ttu-id="ad97e-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="ad97e-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="ad97e-116">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="ad97e-116">[Search for sites][]</span></span>     | <span data-ttu-id="ad97e-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="ad97e-117">GET /sites?search={query}</span></span>

[サイトを取得する]: ../api/site_get.md
[ルート サイトを取得する]: ../api/site_get.md
[パスを使用してサイトを取得する]: ../api/site_getbypath.md
[グループのサイトを取得する]: ../api/site_get.md
[サイトを検索する]: ../api/site_search.md

## <a name="json-representation"></a><span data-ttu-id="ad97e-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad97e-123">JSON representation</span></span>

<span data-ttu-id="ad97e-124">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="ad97e-125">**driveItem** リソースは [**baseItem**](baseitem.md) から派生し、そのリソースからプロパティを継承します。</span><span class="sxs-lookup"><span data-stu-id="ad97e-125">The **driveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource",
       "@odata.type": "microsoft.graph.site",
       "keyProperty": "id",
       "optionalProperties": [ "root", "sharepointIds", "siteCollection", "drive", "drives", "sites" ] } -->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "onenote": [ { "@odata.type": "microsoft.graph.onenote"} ],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="ad97e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad97e-126">Properties</span></span>

| <span data-ttu-id="ad97e-127">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ad97e-127">Property name</span></span>            | <span data-ttu-id="ad97e-128">種類</span><span class="sxs-lookup"><span data-stu-id="ad97e-128">Type</span></span>                                | <span data-ttu-id="ad97e-129">説明</span><span class="sxs-lookup"><span data-stu-id="ad97e-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ad97e-130">**id**</span><span class="sxs-lookup"><span data-stu-id="ad97e-130">**id**</span></span>                   | <span data-ttu-id="ad97e-131">string</span><span class="sxs-lookup"><span data-stu-id="ad97e-131">string</span></span>                              | <span data-ttu-id="ad97e-p101">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="ad97e-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ad97e-134">**createdDateTime**</span></span>      | <span data-ttu-id="ad97e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad97e-135">DateTimeOffset</span></span>                      | <span data-ttu-id="ad97e-p102">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="ad97e-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="ad97e-138">**description**</span></span>          | <span data-ttu-id="ad97e-139">string</span><span class="sxs-lookup"><span data-stu-id="ad97e-139">string</span></span>                              | <span data-ttu-id="ad97e-140">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="ad97e-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="ad97e-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ad97e-141">**displayName**</span></span>          | <span data-ttu-id="ad97e-142">string</span><span class="sxs-lookup"><span data-stu-id="ad97e-142">string</span></span>                              | <span data-ttu-id="ad97e-p103">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="ad97e-145">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ad97e-145">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ad97e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad97e-146">DateTimeOffset</span></span>                      | <span data-ttu-id="ad97e-p104">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p104">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="ad97e-149">**name**</span><span class="sxs-lookup"><span data-stu-id="ad97e-149">**name**</span></span>                 | <span data-ttu-id="ad97e-150">string</span><span class="sxs-lookup"><span data-stu-id="ad97e-150">string</span></span>                              | <span data-ttu-id="ad97e-151">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="ad97e-151">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="ad97e-152">**root**</span><span class="sxs-lookup"><span data-stu-id="ad97e-152">**root**</span></span>                 | [<span data-ttu-id="ad97e-153">root</span><span class="sxs-lookup"><span data-stu-id="ad97e-153">root</span></span>](root.md)                     | <span data-ttu-id="ad97e-p105">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p105">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="ad97e-156">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="ad97e-156">**sharepointIds**</span></span>        | [<span data-ttu-id="ad97e-157">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ad97e-157">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="ad97e-p106">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="ad97e-160">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="ad97e-160">**siteCollection**</span></span>       | [<span data-ttu-id="ad97e-161">siteCollection</span><span class="sxs-lookup"><span data-stu-id="ad97e-161">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="ad97e-p107">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p107">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="ad97e-165">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ad97e-165">**webUrl**</span></span>               | <span data-ttu-id="ad97e-166">string (URL)</span><span class="sxs-lookup"><span data-stu-id="ad97e-166">string (url)</span></span>                        | <span data-ttu-id="ad97e-p108">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p108">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="ad97e-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ad97e-169">Relationships</span></span>

| <span data-ttu-id="ad97e-170">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="ad97e-170">Relationship name</span></span> | <span data-ttu-id="ad97e-171">種類</span><span class="sxs-lookup"><span data-stu-id="ad97e-171">Type</span></span>                             | <span data-ttu-id="ad97e-172">説明</span><span class="sxs-lookup"><span data-stu-id="ad97e-172">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="ad97e-173">**columns**</span><span class="sxs-lookup"><span data-stu-id="ad97e-173">**columns**</span></span>       | <span data-ttu-id="ad97e-174">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ad97e-174">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ad97e-175">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ad97e-175">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="ad97e-176">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ad97e-176"><ContentTypes></span></span>  | <span data-ttu-id="ad97e-177">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ad97e-177">Collection([contentType][])</span></span>      | <span data-ttu-id="ad97e-178">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ad97e-178">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="ad97e-179">**drive**</span><span class="sxs-lookup"><span data-stu-id="ad97e-179">**drive**</span></span>         | <span data-ttu-id="ad97e-180">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="ad97e-180">[drive][]</span></span>                        | <span data-ttu-id="ad97e-181">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="ad97e-181">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="ad97e-182">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="ad97e-182">**drives**</span></span>        | <span data-ttu-id="ad97e-183">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="ad97e-183">Collection([drive][])</span></span>            | <span data-ttu-id="ad97e-184">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="ad97e-184">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="ad97e-185">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="ad97e-185">**items**</span></span>         | <span data-ttu-id="ad97e-186">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="ad97e-186">Collection([baseItem][])</span></span>         | <span data-ttu-id="ad97e-p109">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="ad97e-p109">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ad97e-189">**lists**</span><span class="sxs-lookup"><span data-stu-id="ad97e-189">**Lists**</span></span>         | <span data-ttu-id="ad97e-190">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="ad97e-190">Collection([list][])</span></span>             | <span data-ttu-id="ad97e-191">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ad97e-191">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="ad97e-192">**sites**</span><span class="sxs-lookup"><span data-stu-id="ad97e-192">**sites**</span></span>         | <span data-ttu-id="ad97e-193">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="ad97e-193">Collection([site][])</span></span>             | <span data-ttu-id="ad97e-194">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="ad97e-194">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="ad97e-195">**onenote**</span><span class="sxs-lookup"><span data-stu-id="ad97e-195">**onenote**</span></span>       | <span data-ttu-id="ad97e-196">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="ad97e-196">[onenote][]</span></span>                      | <span data-ttu-id="ad97e-197">ノートブック関連の操作のために OneNote サービスを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="ad97e-197">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
