---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
ms.openlocfilehash: 20d31a9cdc0e540c2b2f2d93fedabdc254e9c03e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265716"
---
# <a name="site-resource"></a><span data-ttu-id="97bf3-102">Site リソース</span><span class="sxs-lookup"><span data-stu-id="97bf3-102">Site resource</span></span>

<span data-ttu-id="97bf3-103">**サイト** リソースは、メタデータと SharePoint サイトのリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="97bf3-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="97bf3-104">タスク</span><span class="sxs-lookup"><span data-stu-id="97bf3-104">Tasks</span></span>

<span data-ttu-id="97bf3-105">以下のすべての例は、`https://graph.microsoft.com/v1.0` からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="97bf3-106">タスク名</span><span class="sxs-lookup"><span data-stu-id="97bf3-106">Task name</span></span>                | <span data-ttu-id="97bf3-107">要求の例</span><span class="sxs-lookup"><span data-stu-id="97bf3-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="97bf3-108">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="97bf3-108">[Get root site][]</span></span>        | <span data-ttu-id="97bf3-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="97bf3-109">GET /sites/root</span></span>
| <span data-ttu-id="97bf3-110">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="97bf3-110">[Get site][]</span></span>             | <span data-ttu-id="97bf3-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="97bf3-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="97bf3-112">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="97bf3-112">[Get site by path][]</span></span>     | <span data-ttu-id="97bf3-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="97bf3-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="97bf3-114">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="97bf3-114">[Get site for a group][]</span></span> | <span data-ttu-id="97bf3-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="97bf3-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="97bf3-116">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="97bf3-116">[Search for sites][]</span></span>     | <span data-ttu-id="97bf3-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="97bf3-117">GET /sites?search={query}</span></span>

[サイトを取得する]: ../api/site_get.md
[Get site]: ../api/site_get.md
[ルート サイトを取得する]: ../api/site_get.md
[Get root site]: ../api/site_get.md
[パスを使用してサイトを取得する]: ../api/site_getbypath.md
[Get site by path]: ../api/site_getbypath.md
[グループのサイトを取得する]: ../api/site_get.md
[Get site for a group]: ../api/site_get.md
[サイトを検索する]: ../api/site_search.md
[Search for sites]: ../api/site_search.md

## <a name="json-representation"></a><span data-ttu-id="97bf3-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97bf3-123">JSON representation</span></span>

<span data-ttu-id="97bf3-124">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="97bf3-125">**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="97bf3-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="97bf3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97bf3-126">Properties</span></span>

| <span data-ttu-id="97bf3-127">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="97bf3-127">Property name</span></span>            | <span data-ttu-id="97bf3-128">型</span><span class="sxs-lookup"><span data-stu-id="97bf3-128">Type</span></span>                                | <span data-ttu-id="97bf3-129">説明</span><span class="sxs-lookup"><span data-stu-id="97bf3-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="97bf3-130">**id**</span><span class="sxs-lookup"><span data-stu-id="97bf3-130">**id**</span></span>                   | <span data-ttu-id="97bf3-131">string</span><span class="sxs-lookup"><span data-stu-id="97bf3-131">string</span></span>                              | <span data-ttu-id="97bf3-p101">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="97bf3-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="97bf3-134">**createdDateTime**</span></span>      | <span data-ttu-id="97bf3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97bf3-135">DateTimeOffset</span></span>                      | <span data-ttu-id="97bf3-p102">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="97bf3-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="97bf3-138">**description**</span></span>          | <span data-ttu-id="97bf3-139">string</span><span class="sxs-lookup"><span data-stu-id="97bf3-139">string</span></span>                              | <span data-ttu-id="97bf3-140">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="97bf3-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="97bf3-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="97bf3-141">**displayName**</span></span>          | <span data-ttu-id="97bf3-142">string</span><span class="sxs-lookup"><span data-stu-id="97bf3-142">string</span></span>                              | <span data-ttu-id="97bf3-p103">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="97bf3-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="97bf3-145">**eTag**</span></span>                 | <span data-ttu-id="97bf3-146">string</span><span class="sxs-lookup"><span data-stu-id="97bf3-146">string</span></span>                              | <span data-ttu-id="97bf3-p104">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="97bf3-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="97bf3-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="97bf3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97bf3-150">DateTimeOffset</span></span>                      | <span data-ttu-id="97bf3-p105">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="97bf3-153">**name**</span><span class="sxs-lookup"><span data-stu-id="97bf3-153">**name**</span></span>                 | <span data-ttu-id="97bf3-154">string</span><span class="sxs-lookup"><span data-stu-id="97bf3-154">string</span></span>                              | <span data-ttu-id="97bf3-155">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="97bf3-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="97bf3-156">**root**</span><span class="sxs-lookup"><span data-stu-id="97bf3-156">**root**</span></span>                 | [<span data-ttu-id="97bf3-157">root</span><span class="sxs-lookup"><span data-stu-id="97bf3-157">root</span></span>](root.md)                     | <span data-ttu-id="97bf3-p106">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="97bf3-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="97bf3-160">**sharepointIds**</span></span>        | [<span data-ttu-id="97bf3-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="97bf3-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="97bf3-p107">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="97bf3-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="97bf3-164">**siteCollection**</span></span>       | [<span data-ttu-id="97bf3-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="97bf3-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="97bf3-p108">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="97bf3-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="97bf3-169">**webUrl**</span></span>               | <span data-ttu-id="97bf3-170">string (URL)</span><span class="sxs-lookup"><span data-stu-id="97bf3-170">string (url)</span></span>                        | <span data-ttu-id="97bf3-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="97bf3-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97bf3-173">Relationships</span></span>

| <span data-ttu-id="97bf3-174">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="97bf3-174">Relationship name</span></span> | <span data-ttu-id="97bf3-175">種類</span><span class="sxs-lookup"><span data-stu-id="97bf3-175">Type</span></span>                             | <span data-ttu-id="97bf3-176">説明</span><span class="sxs-lookup"><span data-stu-id="97bf3-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="97bf3-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="97bf3-177">**columns**</span></span>       | <span data-ttu-id="97bf3-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="97bf3-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="97bf3-179">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="97bf3-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="97bf3-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="97bf3-180">**contentTypes**</span></span>  | <span data-ttu-id="97bf3-181">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="97bf3-181">Collection([contentType][])</span></span>      | <span data-ttu-id="97bf3-182">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="97bf3-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="97bf3-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="97bf3-183">**drive**</span></span>         | <span data-ttu-id="97bf3-184">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="97bf3-184">[drive][]</span></span>                        | <span data-ttu-id="97bf3-185">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="97bf3-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="97bf3-186">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="97bf3-186">**drives**</span></span>        | <span data-ttu-id="97bf3-187">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="97bf3-187">Collection([drive][])</span></span>            | <span data-ttu-id="97bf3-188">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="97bf3-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="97bf3-189">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="97bf3-189">**items**</span></span>         | <span data-ttu-id="97bf3-190">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="97bf3-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="97bf3-p110">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="97bf3-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="97bf3-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="97bf3-193">**lists**</span></span>         | <span data-ttu-id="97bf3-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="97bf3-194">Collection([list][])</span></span>             | <span data-ttu-id="97bf3-195">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="97bf3-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="97bf3-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="97bf3-196">**sites**</span></span>         | <span data-ttu-id="97bf3-197">Collection([サイト][])</span><span class="sxs-lookup"><span data-stu-id="97bf3-197">Collection([site][])</span></span>             | <span data-ttu-id="97bf3-198">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="97bf3-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="97bf3-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="97bf3-199">**onenote**</span></span>       | <span data-ttu-id="97bf3-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="97bf3-200">[onenote][]</span></span>                      | <span data-ttu-id="97bf3-201">ノートブック関連の操作のために OneNote サービスを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="97bf3-201">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
[ドライブ]: drive.md
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
