---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: サイト
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 63d4232c2af37541f2a96359f9d2a209d065bc98
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343060"
---
# <a name="site-resource-type"></a><span data-ttu-id="f16d7-102">サイトのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="f16d7-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f16d7-103">**サイト** リソースは、SharePoint サイトのメタデータとリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="f16d7-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="f16d7-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="f16d7-104">Methods</span></span>

| <span data-ttu-id="f16d7-105">Method</span><span class="sxs-lookup"><span data-stu-id="f16d7-105">Method</span></span>                         | <span data-ttu-id="f16d7-106">REST パス</span><span class="sxs-lookup"><span data-stu-id="f16d7-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="f16d7-107">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-107">[Get root site][]</span></span>              | <span data-ttu-id="f16d7-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="f16d7-108">GET /sites/root</span></span>
| <span data-ttu-id="f16d7-109">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-109">[Get site][]</span></span>                   | <span data-ttu-id="f16d7-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="f16d7-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="f16d7-111">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-111">[Get site by path][]</span></span>           | <span data-ttu-id="f16d7-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="f16d7-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="f16d7-113">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-113">[Get site for a group][]</span></span>       | <span data-ttu-id="f16d7-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="f16d7-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="f16d7-115">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-115">[Get analytics][]</span></span>              | <span data-ttu-id="f16d7-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="f16d7-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="f16d7-117">[間隔によりアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-117">[Get activities by interval][]</span></span> | <span data-ttu-id="f16d7-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="f16d7-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="f16d7-119">[ページを一覧表示する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-119">[List pages][]</span></span>                 | <span data-ttu-id="f16d7-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="f16d7-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="f16d7-121">[ルート サイトを一覧表示する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-121">[List root sites][]</span></span>            | <span data-ttu-id="f16d7-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="f16d7-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="f16d7-123">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-123">[Search for sites][]</span></span>           | <span data-ttu-id="f16d7-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="f16d7-124">GET /sites?search={query}</span></span>

[サイトを取得する]: ../api/site-get.md
[Get site]: ../api/site-get.md
[ルート サイトを取得する]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[パスを使用してサイトを取得する]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[グループのサイトを取得する]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[分析を取得する]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔によりアクティビティを取得する]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[ページを一覧表示する]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[ルート サイトを一覧表示する]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[サイトを検索する]: ../api/site-search.md
[Search for sites]: ../api/site-search.md


## <a name="properties"></a><span data-ttu-id="f16d7-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f16d7-134">Properties</span></span>

| <span data-ttu-id="f16d7-135">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f16d7-135">Property name</span></span>            | <span data-ttu-id="f16d7-136">種類</span><span class="sxs-lookup"><span data-stu-id="f16d7-136">Type</span></span>               | <span data-ttu-id="f16d7-137">説明</span><span class="sxs-lookup"><span data-stu-id="f16d7-137">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="f16d7-138">**id**</span><span class="sxs-lookup"><span data-stu-id="f16d7-138">**id**</span></span>                   | <span data-ttu-id="f16d7-139">string</span><span class="sxs-lookup"><span data-stu-id="f16d7-139">string</span></span>             | <span data-ttu-id="f16d7-p101">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p101">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f16d7-142">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="f16d7-142">**createdDateTime**</span></span>      | <span data-ttu-id="f16d7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f16d7-143">DateTimeOffset</span></span>     | <span data-ttu-id="f16d7-p102">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f16d7-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="f16d7-146">**description**</span></span>          | <span data-ttu-id="f16d7-147">string</span><span class="sxs-lookup"><span data-stu-id="f16d7-147">string</span></span>             | <span data-ttu-id="f16d7-148">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="f16d7-148">The descriptive text for the site.</span></span>
| <span data-ttu-id="f16d7-149">**eTag**</span><span class="sxs-lookup"><span data-stu-id="f16d7-149">**eTag**</span></span>                 | <span data-ttu-id="f16d7-150">string</span><span class="sxs-lookup"><span data-stu-id="f16d7-150">string</span></span>             | <span data-ttu-id="f16d7-p103">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="f16d7-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f16d7-153">**displayName**</span></span>          | <span data-ttu-id="f16d7-154">string</span><span class="sxs-lookup"><span data-stu-id="f16d7-154">string</span></span>             | <span data-ttu-id="f16d7-p104">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="f16d7-157">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f16d7-157">**lastModifiedDateTime**</span></span> | <span data-ttu-id="f16d7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f16d7-158">DateTimeOffset</span></span>     | <span data-ttu-id="f16d7-p105">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f16d7-161">**name**</span><span class="sxs-lookup"><span data-stu-id="f16d7-161">**name**</span></span>                 | <span data-ttu-id="f16d7-162">string</span><span class="sxs-lookup"><span data-stu-id="f16d7-162">string</span></span>             | <span data-ttu-id="f16d7-163">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="f16d7-163">The name / title of the item.</span></span>
| <span data-ttu-id="f16d7-164">**root**</span><span class="sxs-lookup"><span data-stu-id="f16d7-164">**root**</span></span>                 | <span data-ttu-id="f16d7-165">[root][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-165">[root][]</span></span>           | <span data-ttu-id="f16d7-p106">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="f16d7-168">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="f16d7-168">**sharepointIds**</span></span>        | <span data-ttu-id="f16d7-169">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-169">[sharepointIds][]</span></span>  | <span data-ttu-id="f16d7-p107">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f16d7-172">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="f16d7-172">**siteCollection**</span></span>       | <span data-ttu-id="f16d7-173">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-173">[siteCollection][]</span></span> | <span data-ttu-id="f16d7-p108">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="f16d7-177">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="f16d7-177">**webUrl**</span></span>               | <span data-ttu-id="f16d7-178">string (URL)</span><span class="sxs-lookup"><span data-stu-id="f16d7-178">string (url)</span></span>       | <span data-ttu-id="f16d7-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f16d7-181">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f16d7-181">Relationships</span></span>

| <span data-ttu-id="f16d7-182">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="f16d7-182">Relationship name</span></span> | <span data-ttu-id="f16d7-183">種類</span><span class="sxs-lookup"><span data-stu-id="f16d7-183">Type</span></span>                             | <span data-ttu-id="f16d7-184">説明</span><span class="sxs-lookup"><span data-stu-id="f16d7-184">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="f16d7-185">**analytics**</span><span class="sxs-lookup"><span data-stu-id="f16d7-185">**analytics**</span></span>     | <span data-ttu-id="f16d7-186">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="f16d7-186">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="f16d7-187">このサイトで行われたビュー アクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="f16d7-187">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="f16d7-188">**列**</span><span class="sxs-lookup"><span data-stu-id="f16d7-188">**columns**</span></span>       | <span data-ttu-id="f16d7-189">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="f16d7-189">Collection([columnDefinition][])</span></span> | <span data-ttu-id="f16d7-190">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f16d7-190">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="f16d7-191">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="f16d7-191">**contentTypes**</span></span>  | <span data-ttu-id="f16d7-192">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="f16d7-192">Collection([contentType][])</span></span>      | <span data-ttu-id="f16d7-193">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f16d7-193">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="f16d7-194">**drive**</span><span class="sxs-lookup"><span data-stu-id="f16d7-194">**drive**</span></span>         | <span data-ttu-id="f16d7-195">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="f16d7-195">[drive][]</span></span>                        | <span data-ttu-id="f16d7-196">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="f16d7-196">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="f16d7-197">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="f16d7-197">**drives**</span></span>        | <span data-ttu-id="f16d7-198">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="f16d7-198">Collection([drive][])</span></span>            | <span data-ttu-id="f16d7-199">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="f16d7-199">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="f16d7-200">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="f16d7-200">**items**</span></span>         | <span data-ttu-id="f16d7-201">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="f16d7-201">Collection([baseItem][])</span></span>         | <span data-ttu-id="f16d7-p110">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="f16d7-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f16d7-204">**lists**</span><span class="sxs-lookup"><span data-stu-id="f16d7-204">**lists**</span></span>         | <span data-ttu-id="f16d7-205">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="f16d7-205">Collection([list][])</span></span>             | <span data-ttu-id="f16d7-206">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f16d7-206">The collection of lists under this site.</span></span>
| <span data-ttu-id="f16d7-207">**pages**</span><span class="sxs-lookup"><span data-stu-id="f16d7-207">**pages**</span></span>         | <span data-ttu-id="f16d7-208">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="f16d7-208">Collection([sitePage][])</span></span>         | <span data-ttu-id="f16d7-209">このサイトにある SitePages リストのページのコレクション。</span><span class="sxs-lookup"><span data-stu-id="f16d7-209">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="f16d7-210">**sites**</span><span class="sxs-lookup"><span data-stu-id="f16d7-210">**sites**</span></span>         | <span data-ttu-id="f16d7-211">Collection([サイト][])</span><span class="sxs-lookup"><span data-stu-id="f16d7-211">Collection([site][])</span></span>             | <span data-ttu-id="f16d7-212">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="f16d7-212">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="f16d7-224">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f16d7-224">JSON representation</span></span>

<span data-ttu-id="f16d7-225">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f16d7-225">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="f16d7-226">**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="f16d7-226">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": []
}
-->
