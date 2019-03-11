---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d4dfb3f340a2b2b7ff5ad5a3c9279cb2a03c63be
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482092"
---
# <a name="site-resource"></a><span data-ttu-id="36bec-102">Site リソース</span><span class="sxs-lookup"><span data-stu-id="36bec-102">Site resource</span></span>

<span data-ttu-id="36bec-103">**サイト** リソースは、メタデータと SharePoint サイトのリレーションシップを提供します。</span><span class="sxs-lookup"><span data-stu-id="36bec-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="36bec-104">タスク</span><span class="sxs-lookup"><span data-stu-id="36bec-104">Tasks</span></span>

<span data-ttu-id="36bec-105">以下のすべての例は、`https://graph.microsoft.com/v1.0` からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="36bec-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="36bec-106">タスク名</span><span class="sxs-lookup"><span data-stu-id="36bec-106">Task name</span></span>                | <span data-ttu-id="36bec-107">要求の例</span><span class="sxs-lookup"><span data-stu-id="36bec-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="36bec-108">[ルート サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="36bec-108">[Get root site][]</span></span>        | <span data-ttu-id="36bec-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="36bec-109">GET /sites/root</span></span>
| <span data-ttu-id="36bec-110">[サイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="36bec-110">[Get site][]</span></span>             | <span data-ttu-id="36bec-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="36bec-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="36bec-112">[パスを使用してサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="36bec-112">[Get site by path][]</span></span>     | <span data-ttu-id="36bec-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="36bec-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="36bec-114">[グループのサイトを取得する][]</span><span class="sxs-lookup"><span data-stu-id="36bec-114">[Get site for a group][]</span></span> | <span data-ttu-id="36bec-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="36bec-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="36bec-116">[サイトを検索する][]</span><span class="sxs-lookup"><span data-stu-id="36bec-116">[Search for sites][]</span></span>     | <span data-ttu-id="36bec-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="36bec-117">GET /sites?search={query}</span></span>

[サイトを取得する]: ../api/site-get.md
[Get site]: ../api/site-get.md
[ルート サイトを取得する]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[パスを使用してサイトを取得する]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[グループのサイトを取得する]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[サイトを検索する]: ../api/site-search.md
[Search for sites]: ../api/site-search.md

## <a name="json-representation"></a><span data-ttu-id="36bec-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36bec-123">JSON representation</span></span>

<span data-ttu-id="36bec-124">以下は、**サイト** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="36bec-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="36bec-125">**サイト** リソースは [**baseItem**](baseitem.md) から派生しており、そのリソースからプロパティを継承しています。</span><span class="sxs-lookup"><span data-stu-id="36bec-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="36bec-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36bec-126">Properties</span></span>

| <span data-ttu-id="36bec-127">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="36bec-127">Property name</span></span>            | <span data-ttu-id="36bec-128">種類</span><span class="sxs-lookup"><span data-stu-id="36bec-128">Type</span></span>                                | <span data-ttu-id="36bec-129">説明</span><span class="sxs-lookup"><span data-stu-id="36bec-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="36bec-130">**id**</span><span class="sxs-lookup"><span data-stu-id="36bec-130">**id**</span></span>                   | <span data-ttu-id="36bec-131">string</span><span class="sxs-lookup"><span data-stu-id="36bec-131">string</span></span>                              | <span data-ttu-id="36bec-p101">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="36bec-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="36bec-134">**createdDateTime**</span></span>      | <span data-ttu-id="36bec-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36bec-135">DateTimeOffset</span></span>                      | <span data-ttu-id="36bec-p102">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="36bec-138">**説明**</span><span class="sxs-lookup"><span data-stu-id="36bec-138">**description**</span></span>          | <span data-ttu-id="36bec-139">string</span><span class="sxs-lookup"><span data-stu-id="36bec-139">string</span></span>                              | <span data-ttu-id="36bec-140">サイトの説明テキスト。</span><span class="sxs-lookup"><span data-stu-id="36bec-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="36bec-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="36bec-141">**displayName**</span></span>          | <span data-ttu-id="36bec-142">string</span><span class="sxs-lookup"><span data-stu-id="36bec-142">string</span></span>                              | <span data-ttu-id="36bec-p103">サイトの完全なタイトル。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="36bec-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="36bec-145">**eTag**</span></span>                 | <span data-ttu-id="36bec-146">string</span><span class="sxs-lookup"><span data-stu-id="36bec-146">string</span></span>                              | <span data-ttu-id="36bec-p104">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="36bec-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="36bec-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="36bec-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36bec-150">DateTimeOffset</span></span>                      | <span data-ttu-id="36bec-p105">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="36bec-153">**name**</span><span class="sxs-lookup"><span data-stu-id="36bec-153">**name**</span></span>                 | <span data-ttu-id="36bec-154">string</span><span class="sxs-lookup"><span data-stu-id="36bec-154">string</span></span>                              | <span data-ttu-id="36bec-155">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="36bec-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="36bec-156">**root**</span><span class="sxs-lookup"><span data-stu-id="36bec-156">**root**</span></span>                 | [<span data-ttu-id="36bec-157">root</span><span class="sxs-lookup"><span data-stu-id="36bec-157">root</span></span>](root.md)                     | <span data-ttu-id="36bec-p106">存在する場合は、これがサイト コレクションのルート サイトであることを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="36bec-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="36bec-160">**sharepointIds**</span></span>        | [<span data-ttu-id="36bec-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="36bec-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="36bec-p107">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="36bec-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="36bec-164">**siteCollection**</span></span>       | [<span data-ttu-id="36bec-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="36bec-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="36bec-p108">サイトのサイト コレクションに関する詳細情報を提供します。ルート サイトにのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="36bec-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="36bec-169">**webUrl**</span></span>               | <span data-ttu-id="36bec-170">string (URL)</span><span class="sxs-lookup"><span data-stu-id="36bec-170">string (url)</span></span>                        | <span data-ttu-id="36bec-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bec-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="36bec-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="36bec-173">Relationships</span></span>

| <span data-ttu-id="36bec-174">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="36bec-174">Relationship name</span></span> | <span data-ttu-id="36bec-175">種類</span><span class="sxs-lookup"><span data-stu-id="36bec-175">Type</span></span>                             | <span data-ttu-id="36bec-176">説明</span><span class="sxs-lookup"><span data-stu-id="36bec-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="36bec-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="36bec-177">**columns**</span></span>       | <span data-ttu-id="36bec-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="36bec-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="36bec-179">このサイトのすべてのリストで再利用可能なコラム定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="36bec-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="36bec-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="36bec-180">**contentTypes**</span></span>  | <span data-ttu-id="36bec-181">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="36bec-181">Collection([contentType][])</span></span>      | <span data-ttu-id="36bec-182">このサイトに定義されたコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="36bec-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="36bec-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="36bec-183">**drive**</span></span>         | <span data-ttu-id="36bec-184">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="36bec-184">[drive][]</span></span>                        | <span data-ttu-id="36bec-185">このサイトの既定ドライブ (ドキュメント ライブラリ)。</span><span class="sxs-lookup"><span data-stu-id="36bec-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="36bec-186">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="36bec-186">**drives**</span></span>        | <span data-ttu-id="36bec-187">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="36bec-187">Collection([drive][])</span></span>            | <span data-ttu-id="36bec-188">このサイトの下のドライブ (ドキュメント ライブラリ) のコレクション。</span><span class="sxs-lookup"><span data-stu-id="36bec-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="36bec-189">**アイテム**</span><span class="sxs-lookup"><span data-stu-id="36bec-189">**items**</span></span>         | <span data-ttu-id="36bec-190">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="36bec-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="36bec-p110">このサイトに含まれるすべてのアイテムを処理するために使用されました。このコレクションを列挙することはできません。</span><span class="sxs-lookup"><span data-stu-id="36bec-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="36bec-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="36bec-193">**lists**</span></span>         | <span data-ttu-id="36bec-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="36bec-194">Collection([list][])</span></span>             | <span data-ttu-id="36bec-195">このサイトにあるリストのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="36bec-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="36bec-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="36bec-196">**sites**</span></span>         | <span data-ttu-id="36bec-197">Collection([サイト][])</span><span class="sxs-lookup"><span data-stu-id="36bec-197">Collection([site][])</span></span>             | <span data-ttu-id="36bec-198">このサイトの下のサブサイトのコレクション。</span><span class="sxs-lookup"><span data-stu-id="36bec-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="36bec-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="36bec-199">**onenote**</span></span>       | <span data-ttu-id="36bec-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="36bec-200">[onenote][]</span></span>                      | <span data-ttu-id="36bec-201">ノートブック関連の操作のために OneNote サービスを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="36bec-201">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[ドライブ]: drive.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[サイト]: site.md
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
