---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.openlocfilehash: fb91e9bada227f1a22cf862726ea0b6f658fe469
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871023"
---
# <a name="site-resource-type"></a><span data-ttu-id="f9462-102">サイト リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9462-102">site resource type</span></span>

> <span data-ttu-id="f9462-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9462-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9462-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9462-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9462-105">**サイト** リソースは、メタデータと SharePoint サイトのリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="f9462-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="f9462-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f9462-106">Methods</span></span>

| <span data-ttu-id="f9462-107">Method</span><span class="sxs-lookup"><span data-stu-id="f9462-107">Method</span></span>                         | <span data-ttu-id="f9462-108">REST パス</span><span class="sxs-lookup"><span data-stu-id="f9462-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="f9462-109">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f9462-109">[Get root site][]</span></span>              | <span data-ttu-id="f9462-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="f9462-110">GET /sites/root</span></span>
| <span data-ttu-id="f9462-111">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f9462-111">[Get site][]</span></span>                   | <span data-ttu-id="f9462-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="f9462-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="f9462-113">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f9462-113">[Get site by path][]</span></span>           | <span data-ttu-id="f9462-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="f9462-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="f9462-115">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f9462-115">[Get site for a group][]</span></span>       | <span data-ttu-id="f9462-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="f9462-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="f9462-117">[分析を取得します。][]</span><span class="sxs-lookup"><span data-stu-id="f9462-117">[Get analytics][]</span></span>              | <span data-ttu-id="f9462-118">GET/sites/{サイト id}/分析</span><span class="sxs-lookup"><span data-stu-id="f9462-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="f9462-119">[間隔によってアクティビティを取得します。][]</span><span class="sxs-lookup"><span data-stu-id="f9462-119">[Get activities by interval][]</span></span> | <span data-ttu-id="f9462-120">GET/sites/{サイト id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="f9462-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="f9462-121">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="f9462-121">[List pages][]</span></span>                 | <span data-ttu-id="f9462-122">GET/sites/{サイト id} ページ/</span><span class="sxs-lookup"><span data-stu-id="f9462-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="f9462-123">[ルート サイトの一覧][]</span><span class="sxs-lookup"><span data-stu-id="f9462-123">[List root sites][]</span></span>            | <span data-ttu-id="f9462-124">GET/sites ですか? フィルター = null と選択のルート ne = siteCollection、webUrl</span><span class="sxs-lookup"><span data-stu-id="f9462-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="f9462-125">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="f9462-125">[Search for sites][]</span></span>           | <span data-ttu-id="f9462-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="f9462-126">GET /sites?search={query}</span></span>

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


## <a name="properties"></a><span data-ttu-id="f9462-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9462-136">Properties</span></span>

| <span data-ttu-id="f9462-137">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f9462-137">Property name</span></span>            | <span data-ttu-id="f9462-138">Type</span><span class="sxs-lookup"><span data-stu-id="f9462-138">Type</span></span>               | <span data-ttu-id="f9462-139">説明</span><span class="sxs-lookup"><span data-stu-id="f9462-139">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="f9462-140">**id**</span><span class="sxs-lookup"><span data-stu-id="f9462-140">**id**</span></span>                   | <span data-ttu-id="f9462-141">string</span><span class="sxs-lookup"><span data-stu-id="f9462-141">string</span></span>             | <span data-ttu-id="f9462-p102">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f9462-144">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="f9462-144">**createdDateTime**</span></span>      | <span data-ttu-id="f9462-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9462-145">DateTimeOffset</span></span>     | <span data-ttu-id="f9462-p103">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p103">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f9462-148">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9462-148">**description**</span></span>          | <span data-ttu-id="f9462-149">文字列</span><span class="sxs-lookup"><span data-stu-id="f9462-149">string</span></span>             | <span data-ttu-id="f9462-150">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="f9462-150">The descriptive text for the site.</span></span>
| <span data-ttu-id="f9462-151">**eTag**</span><span class="sxs-lookup"><span data-stu-id="f9462-151">**eTag**</span></span>                 | <span data-ttu-id="f9462-152">文字列</span><span class="sxs-lookup"><span data-stu-id="f9462-152">string</span></span>             | <span data-ttu-id="f9462-p104">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="f9462-155">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f9462-155">**displayName**</span></span>          | <span data-ttu-id="f9462-156">文字列</span><span class="sxs-lookup"><span data-stu-id="f9462-156">string</span></span>             | <span data-ttu-id="f9462-p105">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p105">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="f9462-159">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f9462-159">**lastModifiedDateTime**</span></span> | <span data-ttu-id="f9462-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9462-160">DateTimeOffset</span></span>     | <span data-ttu-id="f9462-p106">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p106">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f9462-163">**name**</span><span class="sxs-lookup"><span data-stu-id="f9462-163">**name**</span></span>                 | <span data-ttu-id="f9462-164">文字列</span><span class="sxs-lookup"><span data-stu-id="f9462-164">string</span></span>             | <span data-ttu-id="f9462-165">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="f9462-165">The name / title of the item.</span></span>
| <span data-ttu-id="f9462-166">**root**</span><span class="sxs-lookup"><span data-stu-id="f9462-166">**root**</span></span>                 | <span data-ttu-id="f9462-167">[root][]</span><span class="sxs-lookup"><span data-stu-id="f9462-167">[root][]</span></span>           | <span data-ttu-id="f9462-p107">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p107">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="f9462-170">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="f9462-170">**sharepointIds**</span></span>        | <span data-ttu-id="f9462-171">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f9462-171">[sharepointIds][]</span></span>  | <span data-ttu-id="f9462-p108">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p108">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f9462-174">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="f9462-174">**siteCollection**</span></span>       | <span data-ttu-id="f9462-175">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="f9462-175">[siteCollection][]</span></span> | <span data-ttu-id="f9462-p109">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p109">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="f9462-179">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="f9462-179">**webUrl**</span></span>               | <span data-ttu-id="f9462-180">string (URL)</span><span class="sxs-lookup"><span data-stu-id="f9462-180">string (url)</span></span>       | <span data-ttu-id="f9462-p110">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f9462-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f9462-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f9462-183">Relationships</span></span>

| <span data-ttu-id="f9462-184">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="f9462-184">Relationship name</span></span> | <span data-ttu-id="f9462-185">種類</span><span class="sxs-lookup"><span data-stu-id="f9462-185">Type</span></span>                             | <span data-ttu-id="f9462-186">説明</span><span class="sxs-lookup"><span data-stu-id="f9462-186">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="f9462-187">**分析**</span><span class="sxs-lookup"><span data-stu-id="f9462-187">**analytics**</span></span>     | <span data-ttu-id="f9462-188">[itemAnalytics][]リソース</span><span class="sxs-lookup"><span data-stu-id="f9462-188">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="f9462-189">このサイトで行われた活動の表示について分析します。</span><span class="sxs-lookup"><span data-stu-id="f9462-189">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="f9462-190">**columns**</span><span class="sxs-lookup"><span data-stu-id="f9462-190">**columns**</span></span>       | <span data-ttu-id="f9462-191">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="f9462-191">Collection([columnDefinition][])</span></span> | <span data-ttu-id="f9462-192">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f9462-192">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="f9462-193">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="f9462-193">**contentTypes**</span></span>  | <span data-ttu-id="f9462-194">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="f9462-194">Collection([contentType][])</span></span>      | <span data-ttu-id="f9462-195">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f9462-195">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="f9462-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="f9462-196">**drive**</span></span>         | <span data-ttu-id="f9462-197">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="f9462-197">[drive][]</span></span>                        | <span data-ttu-id="f9462-198">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="f9462-198">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="f9462-199">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="f9462-199">**drives**</span></span>        | <span data-ttu-id="f9462-200">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="f9462-200">Collection([drive][])</span></span>            | <span data-ttu-id="f9462-201">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="f9462-201">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="f9462-202">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="f9462-202">**items**</span></span>         | <span data-ttu-id="f9462-203">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="f9462-203">Collection([baseItem][])</span></span>         | <span data-ttu-id="f9462-p111">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="f9462-p111">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f9462-206">**lists**</span><span class="sxs-lookup"><span data-stu-id="f9462-206">**lists**</span></span>         | <span data-ttu-id="f9462-207">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="f9462-207">Collection([list][])</span></span>             | <span data-ttu-id="f9462-208">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f9462-208">The collection of lists under this site.</span></span>
| <span data-ttu-id="f9462-209">**ページ**</span><span class="sxs-lookup"><span data-stu-id="f9462-209">**pages**</span></span>         | <span data-ttu-id="f9462-210">コレクション ([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="f9462-210">Collection([sitePage][])</span></span>         | <span data-ttu-id="f9462-211">このサイトのサイト ページのリスト内のページのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f9462-211">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="f9462-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="f9462-212">**sites**</span></span>         | <span data-ttu-id="f9462-213">Collection([サイト][])</span><span class="sxs-lookup"><span data-stu-id="f9462-213">Collection([site][])</span></span>             | <span data-ttu-id="f9462-214">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="f9462-214">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="f9462-226">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9462-226">JSON representation</span></span>

<span data-ttu-id="f9462-227">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f9462-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="f9462-228">**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="f9462-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
