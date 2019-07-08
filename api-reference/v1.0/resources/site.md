---
author: JeremyKelley
ms.author: JeremyKelley
title: サイトのリソース
description: サイトのリソースでは、SharePoint サイトのメタデータとリレーションシップを提供します。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 40add99dfbeee28d82b3d02def833497c01385df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968850"
---
# <a name="site-resource"></a><span data-ttu-id="b4c5a-103">サイトのリソース</span><span class="sxs-lookup"><span data-stu-id="b4c5a-103">Site resource</span></span>

<span data-ttu-id="b4c5a-104">**サイト** リソースは、メタデータと SharePoint サイトのリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-104">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="b4c5a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b4c5a-105">Methods</span></span>

| <span data-ttu-id="b4c5a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b4c5a-106">Method</span></span>                | <span data-ttu-id="b4c5a-107">戻り値の種類</span><span class="sxs-lookup"><span data-stu-id="b4c5a-107">Return type</span></span> | <span data-ttu-id="b4c5a-108">説明</span><span class="sxs-lookup"><span data-stu-id="b4c5a-108">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="b4c5a-109">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-109">[Get root site][]</span></span>        | <span data-ttu-id="b4c5a-110">サイト</span><span class="sxs-lookup"><span data-stu-id="b4c5a-110">site</span></span> | <span data-ttu-id="b4c5a-111">テナント内のルートの SharePoint サイトにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-111">To access the root SharePoint site within a tenant:</span></span>
| <span data-ttu-id="b4c5a-112">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-112">[Get site][]</span></span>             | <span data-ttu-id="b4c5a-113">サイト</span><span class="sxs-lookup"><span data-stu-id="b4c5a-113">site</span></span> | <span data-ttu-id="b4c5a-114">SiteId を使用して SharePoint サイトにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-114">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="b4c5a-115">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-115">[Get site by path][]</span></span>     | <span data-ttu-id="b4c5a-116">サイト</span><span class="sxs-lookup"><span data-stu-id="b4c5a-116">site</span></span> | <span data-ttu-id="b4c5a-117">相対パスを使用してルートの SharePoint サイトにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-117">To access the root SharePoint site with a relative path:</span></span>
| <span data-ttu-id="b4c5a-118">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-118">[Get site for a group][]</span></span> | <span data-ttu-id="b4c5a-119">サイト</span><span class="sxs-lookup"><span data-stu-id="b4c5a-119">site</span></span> | <span data-ttu-id="b4c5a-120">グループのチーム サイトにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-120">To access the team site for a group:</span></span>
| <span data-ttu-id="b4c5a-121">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-121">[Get analytics][]</span></span>              | <span data-ttu-id="b4c5a-122">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-122">[itemAnalytics][]</span></span> | <span data-ttu-id="b4c5a-123">このリソースの分析を取得します。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-123">Get analytics for this resource.</span></span> 
| <span data-ttu-id="b4c5a-124">[間隔ごとにアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-124">[Get activities by interval][]</span></span> | <span data-ttu-id="b4c5a-125">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-125">[itemActivityStat][]</span></span> | <span data-ttu-id="b4c5a-126">指定した時間間隔内に**itemActivityStats**のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-126">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="b4c5a-127">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-127">[Search for sites][]</span></span>     | <span data-ttu-id="b4c5a-128">サイトのコレクション</span><span class="sxs-lookup"><span data-stu-id="b4c5a-128">collection of site</span></span> | <span data-ttu-id="b4c5a-129">指定したキーワードと一致するサイトを見つけるために SharePoint のテナント全体を検索します。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-129">Search across a SharePoint tenant for sites that match provided keywords.</span></span>

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
[間隔ごとにアクティビティを取得する]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[サイトを検索する]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md

## <a name="properties"></a><span data-ttu-id="b4c5a-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4c5a-138">Properties</span></span>

| <span data-ttu-id="b4c5a-139">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4c5a-139">Property</span></span>            | <span data-ttu-id="b4c5a-140">型</span><span class="sxs-lookup"><span data-stu-id="b4c5a-140">Type</span></span>                                | <span data-ttu-id="b4c5a-141">説明</span><span class="sxs-lookup"><span data-stu-id="b4c5a-141">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b4c5a-142">**id**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-142">**id**</span></span>                   | <span data-ttu-id="b4c5a-143">string</span><span class="sxs-lookup"><span data-stu-id="b4c5a-143">string</span></span>                              | <span data-ttu-id="b4c5a-p101">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="b4c5a-146">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-146">**createdDateTime**</span></span>      | <span data-ttu-id="b4c5a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c5a-147">DateTimeOffset</span></span>                      | <span data-ttu-id="b4c5a-p102">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="b4c5a-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-150">**description**</span></span>          | <span data-ttu-id="b4c5a-151">string</span><span class="sxs-lookup"><span data-stu-id="b4c5a-151">string</span></span>                              | <span data-ttu-id="b4c5a-152">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-152">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="b4c5a-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-153">**displayName**</span></span>          | <span data-ttu-id="b4c5a-154">string</span><span class="sxs-lookup"><span data-stu-id="b4c5a-154">string</span></span>                              | <span data-ttu-id="b4c5a-p103">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="b4c5a-157">**eTag**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-157">**eTag**</span></span>                 | <span data-ttu-id="b4c5a-158">string</span><span class="sxs-lookup"><span data-stu-id="b4c5a-158">string</span></span>                              | <span data-ttu-id="b4c5a-p104">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="b4c5a-161">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-161">**lastModifiedDateTime**</span></span> | <span data-ttu-id="b4c5a-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c5a-162">DateTimeOffset</span></span>                      | <span data-ttu-id="b4c5a-p105">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="b4c5a-165">**name**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-165">**name**</span></span>                 | <span data-ttu-id="b4c5a-166">string</span><span class="sxs-lookup"><span data-stu-id="b4c5a-166">string</span></span>                              | <span data-ttu-id="b4c5a-167">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-167">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="b4c5a-168">**root**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-168">**root**</span></span>                 | [<span data-ttu-id="b4c5a-169">root</span><span class="sxs-lookup"><span data-stu-id="b4c5a-169">root</span></span>](root.md)                     | <span data-ttu-id="b4c5a-p106">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="b4c5a-172">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-172">**sharepointIds**</span></span>        | [<span data-ttu-id="b4c5a-173">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b4c5a-173">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="b4c5a-p107">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="b4c5a-176">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-176">**siteCollection**</span></span>       | [<span data-ttu-id="b4c5a-177">siteCollection</span><span class="sxs-lookup"><span data-stu-id="b4c5a-177">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="b4c5a-p108">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="b4c5a-181">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-181">**webUrl**</span></span>               | <span data-ttu-id="b4c5a-182">string (URL)</span><span class="sxs-lookup"><span data-stu-id="b4c5a-182">string (url)</span></span>                        | <span data-ttu-id="b4c5a-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="b4c5a-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b4c5a-185">Relationships</span></span>

| <span data-ttu-id="b4c5a-186">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b4c5a-186">Relationship</span></span>      | <span data-ttu-id="b4c5a-187">型</span><span class="sxs-lookup"><span data-stu-id="b4c5a-187">Type</span></span>                             | <span data-ttu-id="b4c5a-188">説明</span><span class="sxs-lookup"><span data-stu-id="b4c5a-188">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="b4c5a-189">**analytics**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-189">**analytics**</span></span>     | <span data-ttu-id="b4c5a-190">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="b4c5a-190">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="b4c5a-191">このサイトで行われたビュー アクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-191">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="b4c5a-192">**列**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-192">**columns**</span></span>       | <span data-ttu-id="b4c5a-193">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="b4c5a-193">Collection([columnDefinition][])</span></span> | <span data-ttu-id="b4c5a-194">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-194">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="b4c5a-195">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-195">**contentTypes**</span></span>  | <span data-ttu-id="b4c5a-196">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="b4c5a-196">Collection([contentType][])</span></span>      | <span data-ttu-id="b4c5a-197">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-197">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="b4c5a-198">**drive**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-198">**drive**</span></span>         | <span data-ttu-id="b4c5a-199">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-199">[drive][]</span></span>                        | <span data-ttu-id="b4c5a-200">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-200">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="b4c5a-201">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-201">**drives**</span></span>        | <span data-ttu-id="b4c5a-202">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="b4c5a-202">Collection([drive][])</span></span>            | <span data-ttu-id="b4c5a-203">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-203">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="b4c5a-204">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-204">**items**</span></span>         | <span data-ttu-id="b4c5a-205">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="b4c5a-205">Collection([baseItem][])</span></span>         | <span data-ttu-id="b4c5a-p110">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="b4c5a-208">**lists**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-208">**lists**</span></span>         | <span data-ttu-id="b4c5a-209">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="b4c5a-209">Collection([list][])</span></span>             | <span data-ttu-id="b4c5a-210">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-210">The collection of lists under this site.</span></span>
| <span data-ttu-id="b4c5a-211">**sites**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-211">**sites**</span></span>         | <span data-ttu-id="b4c5a-212">Collection([サイト][])</span><span class="sxs-lookup"><span data-stu-id="b4c5a-212">Collection([site][])</span></span>             | <span data-ttu-id="b4c5a-213">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-213">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="b4c5a-214">**onenote**</span><span class="sxs-lookup"><span data-stu-id="b4c5a-214">**onenote**</span></span>       | <span data-ttu-id="b4c5a-215">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="b4c5a-215">[onenote][]</span></span>                      | <span data-ttu-id="b4c5a-216">ノートブック関連の操作のために OneNote サービスを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-216">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[リスト]: list.md
[list]: list.md
[サイト]: site.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="b4c5a-225">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4c5a-225">JSON representation</span></span>

<span data-ttu-id="b4c5a-226">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-226">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="b4c5a-227">**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="b4c5a-227">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

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
