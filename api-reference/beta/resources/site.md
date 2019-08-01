---
author: JeremyKelley
description: サイト リソースは、SharePoint サイトのメタデータとリレーションシップを提供します。
ms.date: 09/10/2017
title: サイト
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 691f91b63fdff583476c5308f4b8370a563120a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008356"
---
# <a name="site-resource-type"></a><span data-ttu-id="4fb0b-103">サイトのリソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fb0b-103">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fb0b-104">**サイト** リソースは、SharePoint サイトのメタデータとリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-104">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="4fb0b-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fb0b-105">Methods</span></span>

| <span data-ttu-id="4fb0b-106">Method</span><span class="sxs-lookup"><span data-stu-id="4fb0b-106">Method</span></span>                         | <span data-ttu-id="4fb0b-107">REST パス</span><span class="sxs-lookup"><span data-stu-id="4fb0b-107">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="4fb0b-108">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-108">[Get root site][]</span></span>              | <span data-ttu-id="4fb0b-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="4fb0b-109">GET /sites/root</span></span>
| <span data-ttu-id="4fb0b-110">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-110">[Get site][]</span></span>                   | <span data-ttu-id="4fb0b-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="4fb0b-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="4fb0b-112">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-112">[Get site by path][]</span></span>           | <span data-ttu-id="4fb0b-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="4fb0b-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="4fb0b-114">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-114">[Get site for a group][]</span></span>       | <span data-ttu-id="4fb0b-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="4fb0b-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="4fb0b-116">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-116">[Get analytics][]</span></span>              | <span data-ttu-id="4fb0b-117">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="4fb0b-117">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="4fb0b-118">[間隔によりアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-118">[Get activities by interval][]</span></span> | <span data-ttu-id="4fb0b-119">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="4fb0b-119">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="4fb0b-120">[ページを一覧表示する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-120">[List pages][]</span></span>                 | <span data-ttu-id="4fb0b-121">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="4fb0b-121">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="4fb0b-122">[ルート サイトを一覧表示する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-122">[List root sites][]</span></span>            | <span data-ttu-id="4fb0b-123">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="4fb0b-123">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="4fb0b-124">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-124">[Search for sites][]</span></span>           | <span data-ttu-id="4fb0b-125">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="4fb0b-125">GET /sites?search={query}</span></span>
| <span data-ttu-id="4fb0b-126">[サイトをフォローする][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-126">[Follow Site][]</span></span>                | <span data-ttu-id="4fb0b-127">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="4fb0b-127">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="4fb0b-128">[サイトのフォローを取り消す][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-128">[Unfollow Site][]</span></span>              | <span data-ttu-id="4fb0b-129">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="4fb0b-129">POST /users/{user-id}/followedSites/remove</span></span>

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


## <a name="properties"></a><span data-ttu-id="4fb0b-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb0b-141">Properties</span></span>

| <span data-ttu-id="4fb0b-142">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4fb0b-142">Property name</span></span>            | <span data-ttu-id="4fb0b-143">種類</span><span class="sxs-lookup"><span data-stu-id="4fb0b-143">Type</span></span>               | <span data-ttu-id="4fb0b-144">説明</span><span class="sxs-lookup"><span data-stu-id="4fb0b-144">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="4fb0b-145">**id**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-145">**id**</span></span>                   | <span data-ttu-id="4fb0b-146">文字列</span><span class="sxs-lookup"><span data-stu-id="4fb0b-146">string</span></span>             | <span data-ttu-id="4fb0b-147">アイテムの[一意識別子](#id-property)。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-147">The unique identifier of the item.</span></span> <span data-ttu-id="4fb0b-148">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-148">Read-only.</span></span>
| <span data-ttu-id="4fb0b-149">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-149">**createdDateTime**</span></span>      | <span data-ttu-id="4fb0b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fb0b-150">DateTimeOffset</span></span>     | <span data-ttu-id="4fb0b-p102">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="4fb0b-153">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-153">**description**</span></span>          | <span data-ttu-id="4fb0b-154">string</span><span class="sxs-lookup"><span data-stu-id="4fb0b-154">string</span></span>             | <span data-ttu-id="4fb0b-155">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-155">The descriptive text for the site.</span></span>
| <span data-ttu-id="4fb0b-156">**eTag**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-156">**eTag**</span></span>                 | <span data-ttu-id="4fb0b-157">string</span><span class="sxs-lookup"><span data-stu-id="4fb0b-157">string</span></span>             | <span data-ttu-id="4fb0b-p103">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="4fb0b-160">**displayName**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-160">**displayName**</span></span>          | <span data-ttu-id="4fb0b-161">string</span><span class="sxs-lookup"><span data-stu-id="4fb0b-161">string</span></span>             | <span data-ttu-id="4fb0b-p104">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="4fb0b-164">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-164">**lastModifiedDateTime**</span></span> | <span data-ttu-id="4fb0b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fb0b-165">DateTimeOffset</span></span>     | <span data-ttu-id="4fb0b-p105">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="4fb0b-168">**name**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-168">**name**</span></span>                 | <span data-ttu-id="4fb0b-169">string</span><span class="sxs-lookup"><span data-stu-id="4fb0b-169">string</span></span>             | <span data-ttu-id="4fb0b-170">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-170">The name / title of the item.</span></span>
| <span data-ttu-id="4fb0b-171">**root**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-171">**root**</span></span>                 | <span data-ttu-id="4fb0b-172">[root][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-172">[root][]</span></span>           | <span data-ttu-id="4fb0b-p106">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="4fb0b-175">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-175">**sharepointIds**</span></span>        | <span data-ttu-id="4fb0b-176">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-176">[sharepointIds][]</span></span>  | <span data-ttu-id="4fb0b-p107">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="4fb0b-179">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-179">**siteCollection**</span></span>       | <span data-ttu-id="4fb0b-180">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-180">[siteCollection][]</span></span> | <span data-ttu-id="4fb0b-p108">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="4fb0b-184">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-184">**webUrl**</span></span>               | <span data-ttu-id="4fb0b-185">string (URL)</span><span class="sxs-lookup"><span data-stu-id="4fb0b-185">string (url)</span></span>       | <span data-ttu-id="4fb0b-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="4fb0b-188">ID プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb0b-188">id property</span></span>
<span data-ttu-id="4fb0b-189">**サイト**は、次の値の複合である一意な ID によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-189">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>
* <span data-ttu-id="4fb0b-190">サイト コレクションのホスト名 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="4fb0b-190">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="4fb0b-191">サイト コレクションの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="4fb0b-191">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="4fb0b-192">サイトの一意 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="4fb0b-192">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="4fb0b-193">`root` 識別子は次に示すように、常にターゲットのルート サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-193">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="4fb0b-194">`/sites/root`:テナントのルート サイト。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-194">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="4fb0b-195">`/groups/{group-id}/sites/root`:グループのチーム サイト。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-195">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="4fb0b-196">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fb0b-196">Relationships</span></span>

| <span data-ttu-id="4fb0b-197">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="4fb0b-197">Relationship name</span></span> | <span data-ttu-id="4fb0b-198">種類</span><span class="sxs-lookup"><span data-stu-id="4fb0b-198">Type</span></span>                             | <span data-ttu-id="4fb0b-199">説明</span><span class="sxs-lookup"><span data-stu-id="4fb0b-199">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="4fb0b-200">**analytics**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-200">**analytics**</span></span>     | <span data-ttu-id="4fb0b-201">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="4fb0b-201">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="4fb0b-202">このサイトで行われたビュー アクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-202">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="4fb0b-203">**列**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-203">**columns**</span></span>       | <span data-ttu-id="4fb0b-204">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="4fb0b-204">Collection([columnDefinition][])</span></span> | <span data-ttu-id="4fb0b-205">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-205">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="4fb0b-206">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-206">**contentTypes**</span></span>  | <span data-ttu-id="4fb0b-207">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="4fb0b-207">Collection([contentType][])</span></span>      | <span data-ttu-id="4fb0b-208">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-208">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="4fb0b-209">**drive**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-209">**drive**</span></span>         | <span data-ttu-id="4fb0b-210">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="4fb0b-210">[drive][]</span></span>                        | <span data-ttu-id="4fb0b-211">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-211">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="4fb0b-212">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-212">**drives**</span></span>        | <span data-ttu-id="4fb0b-213">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="4fb0b-213">Collection([drive][])</span></span>            | <span data-ttu-id="4fb0b-214">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-214">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="4fb0b-215">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-215">**items**</span></span>         | <span data-ttu-id="4fb0b-216">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="4fb0b-216">Collection([baseItem][])</span></span>         | <span data-ttu-id="4fb0b-p110">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="4fb0b-219">**lists**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-219">**lists**</span></span>         | <span data-ttu-id="4fb0b-220">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="4fb0b-220">Collection([list][])</span></span>             | <span data-ttu-id="4fb0b-221">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-221">The collection of lists under this site.</span></span>
| <span data-ttu-id="4fb0b-222">**pages**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-222">**pages**</span></span>         | <span data-ttu-id="4fb0b-223">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="4fb0b-223">Collection([sitePage][])</span></span>         | <span data-ttu-id="4fb0b-224">このサイトにある SitePages リストのページのコレクション。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-224">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="4fb0b-225">**sites**</span><span class="sxs-lookup"><span data-stu-id="4fb0b-225">**sites**</span></span>         | <span data-ttu-id="4fb0b-226">Collection([サイト][])</span><span class="sxs-lookup"><span data-stu-id="4fb0b-226">Collection([site][])</span></span>             | <span data-ttu-id="4fb0b-227">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-227">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="4fb0b-239">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4fb0b-239">JSON representation</span></span>

<span data-ttu-id="4fb0b-240">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-240">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="4fb0b-241">**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="4fb0b-241">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
