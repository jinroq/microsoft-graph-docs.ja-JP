---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1676a314b7c1283918518655b3180cbc70ca193e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952350"
---
# <a name="site-resource-type"></a><span data-ttu-id="55576-102">サイト リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55576-102">site resource type</span></span>

> <span data-ttu-id="55576-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="55576-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55576-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55576-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55576-105">**サイト** リソースは、メタデータと SharePoint サイトのリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="55576-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="55576-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="55576-106">Methods</span></span>

| <span data-ttu-id="55576-107">Method</span><span class="sxs-lookup"><span data-stu-id="55576-107">Method</span></span>                         | <span data-ttu-id="55576-108">REST パス</span><span class="sxs-lookup"><span data-stu-id="55576-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="55576-109">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="55576-109">[Get root site][]</span></span>              | <span data-ttu-id="55576-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="55576-110">GET /sites/root</span></span>
| <span data-ttu-id="55576-111">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="55576-111">[Get site][]</span></span>                   | <span data-ttu-id="55576-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="55576-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="55576-113">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="55576-113">[Get site by path][]</span></span>           | <span data-ttu-id="55576-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="55576-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="55576-115">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="55576-115">[Get site for a group][]</span></span>       | <span data-ttu-id="55576-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="55576-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="55576-117">[分析を取得します。][]</span><span class="sxs-lookup"><span data-stu-id="55576-117">[Get analytics][]</span></span>              | <span data-ttu-id="55576-118">GET/sites/{サイト id}/分析</span><span class="sxs-lookup"><span data-stu-id="55576-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="55576-119">[間隔によってアクティビティを取得します。][]</span><span class="sxs-lookup"><span data-stu-id="55576-119">[Get activities by interval][]</span></span> | <span data-ttu-id="55576-120">GET/sites/{サイト id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="55576-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="55576-121">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="55576-121">[List pages][]</span></span>                 | <span data-ttu-id="55576-122">GET/sites/{サイト id} ページ/</span><span class="sxs-lookup"><span data-stu-id="55576-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="55576-123">[ルート サイトの一覧][]</span><span class="sxs-lookup"><span data-stu-id="55576-123">[List root sites][]</span></span>            | <span data-ttu-id="55576-124">GET/sites ですか? フィルター = null と選択のルート ne = siteCollection、webUrl</span><span class="sxs-lookup"><span data-stu-id="55576-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="55576-125">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="55576-125">[Search for sites][]</span></span>           | <span data-ttu-id="55576-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="55576-126">GET /sites?search={query}</span></span>

[サイトを取得する]: ../api/site-get.md
[Get site]: ../api/site-get.md
[ルート サイトを取得する]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[パスを使用してサイトを取得する]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[グループのサイトを取得する]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[分析を取得します。]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔によってアクティビティを取得します。]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[List pages]: ../api/sitepage-list.md
[ルート サイトの一覧]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[サイトを検索する]: ../api/site-search.md
[Search for sites]: ../api/site-search.md


## <a name="properties"></a><span data-ttu-id="55576-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55576-136">Properties</span></span>

| <span data-ttu-id="55576-137">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="55576-137">Property name</span></span>            | <span data-ttu-id="55576-138">Type</span><span class="sxs-lookup"><span data-stu-id="55576-138">Type</span></span>               | <span data-ttu-id="55576-139">説明</span><span class="sxs-lookup"><span data-stu-id="55576-139">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="55576-140">**id**</span><span class="sxs-lookup"><span data-stu-id="55576-140">**id**</span></span>                   | <span data-ttu-id="55576-141">string</span><span class="sxs-lookup"><span data-stu-id="55576-141">string</span></span>             | <span data-ttu-id="55576-p102">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="55576-144">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="55576-144">**createdDateTime**</span></span>      | <span data-ttu-id="55576-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55576-145">DateTimeOffset</span></span>     | <span data-ttu-id="55576-p103">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p103">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="55576-148">**説明**</span><span class="sxs-lookup"><span data-stu-id="55576-148">**description**</span></span>          | <span data-ttu-id="55576-149">文字列</span><span class="sxs-lookup"><span data-stu-id="55576-149">string</span></span>             | <span data-ttu-id="55576-150">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="55576-150">The descriptive text for the site.</span></span>
| <span data-ttu-id="55576-151">**eTag**</span><span class="sxs-lookup"><span data-stu-id="55576-151">**eTag**</span></span>                 | <span data-ttu-id="55576-152">文字列</span><span class="sxs-lookup"><span data-stu-id="55576-152">string</span></span>             | <span data-ttu-id="55576-p104">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="55576-155">**displayName**</span><span class="sxs-lookup"><span data-stu-id="55576-155">**displayName**</span></span>          | <span data-ttu-id="55576-156">文字列</span><span class="sxs-lookup"><span data-stu-id="55576-156">string</span></span>             | <span data-ttu-id="55576-p105">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p105">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="55576-159">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="55576-159">**lastModifiedDateTime**</span></span> | <span data-ttu-id="55576-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55576-160">DateTimeOffset</span></span>     | <span data-ttu-id="55576-p106">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p106">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="55576-163">**name**</span><span class="sxs-lookup"><span data-stu-id="55576-163">**name**</span></span>                 | <span data-ttu-id="55576-164">文字列</span><span class="sxs-lookup"><span data-stu-id="55576-164">string</span></span>             | <span data-ttu-id="55576-165">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="55576-165">The name / title of the item.</span></span>
| <span data-ttu-id="55576-166">**root**</span><span class="sxs-lookup"><span data-stu-id="55576-166">**root**</span></span>                 | <span data-ttu-id="55576-167">[root][]</span><span class="sxs-lookup"><span data-stu-id="55576-167">[root][]</span></span>           | <span data-ttu-id="55576-p107">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p107">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="55576-170">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="55576-170">**sharepointIds**</span></span>        | <span data-ttu-id="55576-171">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="55576-171">[sharepointIds][]</span></span>  | <span data-ttu-id="55576-p108">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p108">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="55576-174">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="55576-174">**siteCollection**</span></span>       | <span data-ttu-id="55576-175">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="55576-175">[siteCollection][]</span></span> | <span data-ttu-id="55576-p109">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p109">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="55576-179">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="55576-179">**webUrl**</span></span>               | <span data-ttu-id="55576-180">string (URL)</span><span class="sxs-lookup"><span data-stu-id="55576-180">string (url)</span></span>       | <span data-ttu-id="55576-p110">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55576-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="55576-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="55576-183">Relationships</span></span>

| <span data-ttu-id="55576-184">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="55576-184">Relationship name</span></span> | <span data-ttu-id="55576-185">種類</span><span class="sxs-lookup"><span data-stu-id="55576-185">Type</span></span>                             | <span data-ttu-id="55576-186">説明</span><span class="sxs-lookup"><span data-stu-id="55576-186">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="55576-187">**分析**</span><span class="sxs-lookup"><span data-stu-id="55576-187">**analytics**</span></span>     | <span data-ttu-id="55576-188">[itemAnalytics][]リソース</span><span class="sxs-lookup"><span data-stu-id="55576-188">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="55576-189">このサイトで行われた活動の表示について分析します。</span><span class="sxs-lookup"><span data-stu-id="55576-189">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="55576-190">**columns**</span><span class="sxs-lookup"><span data-stu-id="55576-190">**columns**</span></span>       | <span data-ttu-id="55576-191">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="55576-191">Collection([columnDefinition][])</span></span> | <span data-ttu-id="55576-192">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="55576-192">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="55576-193">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="55576-193">**contentTypes**</span></span>  | <span data-ttu-id="55576-194">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="55576-194">Collection([contentType][])</span></span>      | <span data-ttu-id="55576-195">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="55576-195">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="55576-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="55576-196">**drive**</span></span>         | <span data-ttu-id="55576-197">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="55576-197">[drive][]</span></span>                        | <span data-ttu-id="55576-198">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="55576-198">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="55576-199">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="55576-199">**drives**</span></span>        | <span data-ttu-id="55576-200">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="55576-200">Collection([drive][])</span></span>            | <span data-ttu-id="55576-201">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="55576-201">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="55576-202">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="55576-202">**items**</span></span>         | <span data-ttu-id="55576-203">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="55576-203">Collection([baseItem][])</span></span>         | <span data-ttu-id="55576-p111">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="55576-p111">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="55576-206">**lists**</span><span class="sxs-lookup"><span data-stu-id="55576-206">**lists**</span></span>         | <span data-ttu-id="55576-207">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="55576-207">Collection([list][])</span></span>             | <span data-ttu-id="55576-208">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="55576-208">The collection of lists under this site.</span></span>
| <span data-ttu-id="55576-209">**ページ**</span><span class="sxs-lookup"><span data-stu-id="55576-209">**pages**</span></span>         | <span data-ttu-id="55576-210">コレクション ([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="55576-210">Collection([sitePage][])</span></span>         | <span data-ttu-id="55576-211">このサイトのサイト ページのリスト内のページのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="55576-211">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="55576-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="55576-212">**sites**</span></span>         | <span data-ttu-id="55576-213">Collection([サイト][])</span><span class="sxs-lookup"><span data-stu-id="55576-213">Collection([site][])</span></span>             | <span data-ttu-id="55576-214">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="55576-214">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[ドライブ]: drive.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[リスト]: list.md
[list]: list.md
[sitePage]: sitepage.md
[ルート]: root.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="55576-226">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55576-226">JSON representation</span></span>

<span data-ttu-id="55576-227">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="55576-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="55576-228">**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="55576-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
