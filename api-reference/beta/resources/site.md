---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: サイト
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f2386228c3758cc15d9c270f0da32608e4f2b901
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683504"
---
# <a name="site-resource-type"></a><span data-ttu-id="4667e-102">サイトのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="4667e-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4667e-103">**サイト** リソースは、SharePoint サイトのメタデータとリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="4667e-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="4667e-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="4667e-104">Methods</span></span>

| <span data-ttu-id="4667e-105">Method</span><span class="sxs-lookup"><span data-stu-id="4667e-105">Method</span></span>                         | <span data-ttu-id="4667e-106">REST パス</span><span class="sxs-lookup"><span data-stu-id="4667e-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="4667e-107">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-107">[Get root site][]</span></span>              | <span data-ttu-id="4667e-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="4667e-108">GET /sites/root</span></span>
| <span data-ttu-id="4667e-109">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-109">[Get site][]</span></span>                   | <span data-ttu-id="4667e-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="4667e-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="4667e-111">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-111">[Get site by path][]</span></span>           | <span data-ttu-id="4667e-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="4667e-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="4667e-113">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-113">[Get site for a group][]</span></span>       | <span data-ttu-id="4667e-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="4667e-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="4667e-115">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-115">[Get analytics][]</span></span>              | <span data-ttu-id="4667e-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="4667e-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="4667e-117">[間隔によりアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-117">[Get activities by interval][]</span></span> | <span data-ttu-id="4667e-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="4667e-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="4667e-119">[ページを一覧表示する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-119">[List pages][]</span></span>                 | <span data-ttu-id="4667e-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="4667e-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="4667e-121">[ルート サイトを一覧表示する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-121">[List root sites][]</span></span>            | <span data-ttu-id="4667e-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="4667e-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="4667e-123">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="4667e-123">[Search for sites][]</span></span>           | <span data-ttu-id="4667e-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="4667e-124">GET /sites?search={query}</span></span>
| <span data-ttu-id="4667e-125">[サイトをフォローする][]</span><span class="sxs-lookup"><span data-stu-id="4667e-125">[Follow Site][]</span></span>                | <span data-ttu-id="4667e-126">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="4667e-126">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="4667e-127">[サイトのフォローを取り消す][]</span><span class="sxs-lookup"><span data-stu-id="4667e-127">[Unfollow Site][]</span></span>              | <span data-ttu-id="4667e-128">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="4667e-128">POST /users/{user-id}/followedSites/remove</span></span>

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
[サイトをフォローする]: ../api/site-follow.md
[Follow site]: ../api/site-follow.md
[サイトのフォローを取り消す]: ../api/site-unfollow.md
[Unfollow site]: ../api/site-unfollow.md


## <a name="properties"></a><span data-ttu-id="4667e-140">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4667e-140">Properties</span></span>

| <span data-ttu-id="4667e-141">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4667e-141">Property name</span></span>            | <span data-ttu-id="4667e-142">種類</span><span class="sxs-lookup"><span data-stu-id="4667e-142">Type</span></span>               | <span data-ttu-id="4667e-143">説明</span><span class="sxs-lookup"><span data-stu-id="4667e-143">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="4667e-144">**id**</span><span class="sxs-lookup"><span data-stu-id="4667e-144">**id**</span></span>                   | <span data-ttu-id="4667e-145">文字列</span><span class="sxs-lookup"><span data-stu-id="4667e-145">string</span></span>             | <span data-ttu-id="4667e-146">アイテムの[一意識別子](#id-property)。</span><span class="sxs-lookup"><span data-stu-id="4667e-146">The unique identifier of the item.</span></span> <span data-ttu-id="4667e-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-147">Read-only.</span></span>
| <span data-ttu-id="4667e-148">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="4667e-148">**createdDateTime**</span></span>      | <span data-ttu-id="4667e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4667e-149">DateTimeOffset</span></span>     | <span data-ttu-id="4667e-p102">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="4667e-152">**説明**</span><span class="sxs-lookup"><span data-stu-id="4667e-152">**description**</span></span>          | <span data-ttu-id="4667e-153">string</span><span class="sxs-lookup"><span data-stu-id="4667e-153">string</span></span>             | <span data-ttu-id="4667e-154">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="4667e-154">The descriptive text for the site.</span></span>
| <span data-ttu-id="4667e-155">**eTag**</span><span class="sxs-lookup"><span data-stu-id="4667e-155">**eTag**</span></span>                 | <span data-ttu-id="4667e-156">string</span><span class="sxs-lookup"><span data-stu-id="4667e-156">string</span></span>             | <span data-ttu-id="4667e-p103">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="4667e-159">**displayName**</span><span class="sxs-lookup"><span data-stu-id="4667e-159">**displayName**</span></span>          | <span data-ttu-id="4667e-160">string</span><span class="sxs-lookup"><span data-stu-id="4667e-160">string</span></span>             | <span data-ttu-id="4667e-p104">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="4667e-163">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="4667e-163">**lastModifiedDateTime**</span></span> | <span data-ttu-id="4667e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4667e-164">DateTimeOffset</span></span>     | <span data-ttu-id="4667e-p105">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="4667e-167">**name**</span><span class="sxs-lookup"><span data-stu-id="4667e-167">**name**</span></span>                 | <span data-ttu-id="4667e-168">string</span><span class="sxs-lookup"><span data-stu-id="4667e-168">string</span></span>             | <span data-ttu-id="4667e-169">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="4667e-169">The name / title of the item.</span></span>
| <span data-ttu-id="4667e-170">**root**</span><span class="sxs-lookup"><span data-stu-id="4667e-170">**root**</span></span>                 | <span data-ttu-id="4667e-171">[root][]</span><span class="sxs-lookup"><span data-stu-id="4667e-171">[root][]</span></span>           | <span data-ttu-id="4667e-p106">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="4667e-174">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="4667e-174">**sharepointIds**</span></span>        | <span data-ttu-id="4667e-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4667e-175">[sharepointIds][]</span></span>  | <span data-ttu-id="4667e-p107">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="4667e-178">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="4667e-178">**siteCollection**</span></span>       | <span data-ttu-id="4667e-179">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="4667e-179">[siteCollection][]</span></span> | <span data-ttu-id="4667e-p108">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="4667e-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="4667e-183">**webUrl**</span></span>               | <span data-ttu-id="4667e-184">string (URL)</span><span class="sxs-lookup"><span data-stu-id="4667e-184">string (url)</span></span>       | <span data-ttu-id="4667e-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4667e-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="4667e-187">ID プロパティ</span><span class="sxs-lookup"><span data-stu-id="4667e-187">id property</span></span>
<span data-ttu-id="4667e-188">**サイト**は、次の値の複合である一意な ID によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="4667e-188">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>
* <span data-ttu-id="4667e-189">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="4667e-189">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="4667e-190">サイト コレクションの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="4667e-190">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="4667e-191">サイトの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="4667e-191">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="4667e-192">`root` 識別子は次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="4667e-192">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="4667e-193">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="4667e-193">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="4667e-194">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="4667e-194">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="4667e-195">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4667e-195">Relationships</span></span>

| <span data-ttu-id="4667e-196">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="4667e-196">Relationship name</span></span> | <span data-ttu-id="4667e-197">種類</span><span class="sxs-lookup"><span data-stu-id="4667e-197">Type</span></span>                             | <span data-ttu-id="4667e-198">説明</span><span class="sxs-lookup"><span data-stu-id="4667e-198">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="4667e-199">**analytics**</span><span class="sxs-lookup"><span data-stu-id="4667e-199">**analytics**</span></span>     | <span data-ttu-id="4667e-200">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="4667e-200">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="4667e-201">このサイトで行われたビュー アクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="4667e-201">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="4667e-202">**列**</span><span class="sxs-lookup"><span data-stu-id="4667e-202">**columns**</span></span>       | <span data-ttu-id="4667e-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="4667e-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="4667e-204">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4667e-204">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="4667e-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="4667e-205">**contentTypes**</span></span>  | <span data-ttu-id="4667e-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="4667e-206">Collection([contentType][])</span></span>      | <span data-ttu-id="4667e-207">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4667e-207">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="4667e-208">**drive**</span><span class="sxs-lookup"><span data-stu-id="4667e-208">**drive**</span></span>         | <span data-ttu-id="4667e-209">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="4667e-209">[drive][]</span></span>                        | <span data-ttu-id="4667e-210">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="4667e-210">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="4667e-211">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="4667e-211">**drives**</span></span>        | <span data-ttu-id="4667e-212">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="4667e-212">Collection([drive][])</span></span>            | <span data-ttu-id="4667e-213">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="4667e-213">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="4667e-214">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="4667e-214">**items**</span></span>         | <span data-ttu-id="4667e-215">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="4667e-215">Collection([baseItem][])</span></span>         | <span data-ttu-id="4667e-p110">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="4667e-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="4667e-218">**lists**</span><span class="sxs-lookup"><span data-stu-id="4667e-218">**lists**</span></span>         | <span data-ttu-id="4667e-219">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="4667e-219">Collection([list][])</span></span>             | <span data-ttu-id="4667e-220">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4667e-220">The collection of lists under this site.</span></span>
| <span data-ttu-id="4667e-221">**pages**</span><span class="sxs-lookup"><span data-stu-id="4667e-221">**pages**</span></span>         | <span data-ttu-id="4667e-222">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="4667e-222">Collection([sitePage][])</span></span>         | <span data-ttu-id="4667e-223">このサイトにある SitePages リストのページのコレクション。</span><span class="sxs-lookup"><span data-stu-id="4667e-223">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="4667e-224">**sites**</span><span class="sxs-lookup"><span data-stu-id="4667e-224">**sites**</span></span>         | <span data-ttu-id="4667e-225">Collection([サイト][])</span><span class="sxs-lookup"><span data-stu-id="4667e-225">Collection([site][])</span></span>             | <span data-ttu-id="4667e-226">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="4667e-226">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="4667e-238">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4667e-238">JSON representation</span></span>

<span data-ttu-id="4667e-239">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4667e-239">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="4667e-240">**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="4667e-240">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
