---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a756929212dbca04f16e9e4701e34bbd8d4de28f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939239"
---
# <a name="sitepage-resource"></a><span data-ttu-id="df399-102">sitePage リソース</span><span class="sxs-lookup"><span data-stu-id="df399-102">sitePage resource</span></span>

> <span data-ttu-id="df399-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df399-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df399-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df399-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df399-105">このリソースは、サイト ページの[一覧][]でページを表します。</span><span class="sxs-lookup"><span data-stu-id="df399-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="df399-106">タイトル、レイアウト、および[web パーツ][]の s のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="df399-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="df399-107">ページ上のタスク</span><span class="sxs-lookup"><span data-stu-id="df399-107">Tasks on a page</span></span>

<span data-ttu-id="df399-108">**SitePage**リソースの次のタスクを利用できます。</span><span class="sxs-lookup"><span data-stu-id="df399-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="df399-109">以下のすべての例は、[サイト][]では、例えば: `https://graph.microsoft.com/{api-version}/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="df399-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="df399-110">共通タスク</span><span class="sxs-lookup"><span data-stu-id="df399-110">Common task</span></span>                     | <span data-ttu-id="df399-111">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="df399-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="df399-112">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="df399-112">[List pages][]</span></span>                  | <span data-ttu-id="df399-113">/Pages を取得します。</span><span class="sxs-lookup"><span data-stu-id="df399-113">GET /pages</span></span>
| <span data-ttu-id="df399-114">[Get page][]</span><span class="sxs-lookup"><span data-stu-id="df399-114">[Get page][]</span></span>                    | <span data-ttu-id="df399-115">/Pages/{ページの id を取得します。</span><span class="sxs-lookup"><span data-stu-id="df399-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="df399-116">[Create][]</span><span class="sxs-lookup"><span data-stu-id="df399-116">[Create][]</span></span>                      | <span data-ttu-id="df399-117">投稿/pages</span><span class="sxs-lookup"><span data-stu-id="df399-117">POST /pages</span></span>
| <span data-ttu-id="df399-118">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="df399-118">[Delete][]</span></span>                      | <span data-ttu-id="df399-119">/Pages/{ページの id を削除します。</span><span class="sxs-lookup"><span data-stu-id="df399-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="df399-120">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="df399-120">[Publish][]</span></span>                     | <span data-ttu-id="df399-121">/Pages/{ページ id} の投稿し、公開</span><span class="sxs-lookup"><span data-stu-id="df399-121">POST /pages/{page-id}/publish</span></span>

[List pages]: ../api/sitepage-list.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="df399-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df399-127">JSON representation</span></span>

<span data-ttu-id="df399-128">ここでは、 **sitePage**リソースの JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="df399-128">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="df399-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df399-129">Properties</span></span>

<span data-ttu-id="df399-130">**SitePage**リソースでは、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="df399-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="df399-131">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="df399-131">Property name</span></span>    | <span data-ttu-id="df399-132">型</span><span class="sxs-lookup"><span data-stu-id="df399-132">Type</span></span>                         | <span data-ttu-id="df399-133">説明</span><span class="sxs-lookup"><span data-stu-id="df399-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="df399-134">contentType</span><span class="sxs-lookup"><span data-stu-id="df399-134">contentType</span></span>      | <span data-ttu-id="df399-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="df399-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="df399-136">ページのコンテンツの種類です。</span><span class="sxs-lookup"><span data-stu-id="df399-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="df399-137">ページのコンテンツ</span><span class="sxs-lookup"><span data-stu-id="df399-137">Page Content</span></span>

<span data-ttu-id="df399-138">**SitePage**リソースでは、次のコンテンツのフィールドがあります。</span><span class="sxs-lookup"><span data-stu-id="df399-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="df399-139">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="df399-139">Property name</span></span>      | <span data-ttu-id="df399-140">型</span><span class="sxs-lookup"><span data-stu-id="df399-140">Type</span></span>                       | <span data-ttu-id="df399-141">説明</span><span class="sxs-lookup"><span data-stu-id="df399-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="df399-142">タイトル</span><span class="sxs-lookup"><span data-stu-id="df399-142">title</span></span>              | <span data-ttu-id="df399-143">文字列</span><span class="sxs-lookup"><span data-stu-id="df399-143">string</span></span>                     | <span data-ttu-id="df399-144">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="df399-144">The title of the page.</span></span>
| <span data-ttu-id="df399-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="df399-145">pageLayout</span></span>         | <span data-ttu-id="df399-146">文字列</span><span class="sxs-lookup"><span data-stu-id="df399-146">string</span></span>                     | <span data-ttu-id="df399-147">ページのページ レイアウトの名前。</span><span class="sxs-lookup"><span data-stu-id="df399-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="df399-148">web パーツ</span><span class="sxs-lookup"><span data-stu-id="df399-148">webParts</span></span>           | <span data-ttu-id="df399-149">[web パーツ][]</span><span class="sxs-lookup"><span data-stu-id="df399-149">[webPart][]</span></span>                | <span data-ttu-id="df399-150">ページ上の web パーツです。</span><span class="sxs-lookup"><span data-stu-id="df399-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="df399-151">メタデータを作成する</span><span class="sxs-lookup"><span data-stu-id="df399-151">Authoring Metadata</span></span>

<span data-ttu-id="df399-152">**SitePage**のリソースには、次の作成に関連するメタデータがあります。</span><span class="sxs-lookup"><span data-stu-id="df399-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="df399-153">PublishingState プロパティは、このようなチェック アウトされているか、公開の状態を作成するページに反映されます。</span><span class="sxs-lookup"><span data-stu-id="df399-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="df399-154">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="df399-154">Property name</span></span>          | <span data-ttu-id="df399-155">型</span><span class="sxs-lookup"><span data-stu-id="df399-155">Type</span></span>                   | <span data-ttu-id="df399-156">説明</span><span class="sxs-lookup"><span data-stu-id="df399-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="df399-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="df399-157">publishingState</span></span>        | <span data-ttu-id="df399-158">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="df399-158">[publicationFacet][]</span></span>   | <span data-ttu-id="df399-159">発行のステータスと MM.mm バージョンのページです。</span><span class="sxs-lookup"><span data-stu-id="df399-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="df399-160">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="df399-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="df399-161">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="df399-161">Property name</span></span>        | <span data-ttu-id="df399-162">型</span><span class="sxs-lookup"><span data-stu-id="df399-162">Type</span></span>              | <span data-ttu-id="df399-163">説明</span><span class="sxs-lookup"><span data-stu-id="df399-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="df399-164">ID</span><span class="sxs-lookup"><span data-stu-id="df399-164">id</span></span>                   | <span data-ttu-id="df399-165">文字列</span><span class="sxs-lookup"><span data-stu-id="df399-165">string</span></span>            | <span data-ttu-id="df399-p105">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="df399-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="df399-168">name</span><span class="sxs-lookup"><span data-stu-id="df399-168">name</span></span>                 | <span data-ttu-id="df399-169">文字列</span><span class="sxs-lookup"><span data-stu-id="df399-169">string</span></span>            | <span data-ttu-id="df399-170">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="df399-170">The name / title of the item.</span></span>
| <span data-ttu-id="df399-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="df399-171">createdBy</span></span>            | <span data-ttu-id="df399-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="df399-172">[identitySet][]</span></span>   | <span data-ttu-id="df399-173">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="df399-173">Identity of the creator of this item.</span></span> <span data-ttu-id="df399-174">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="df399-174">Read-only.</span></span>
| <span data-ttu-id="df399-175">eTag</span><span class="sxs-lookup"><span data-stu-id="df399-175">eTag</span></span>                 | <span data-ttu-id="df399-176">文字列</span><span class="sxs-lookup"><span data-stu-id="df399-176">string</span></span>            | <span data-ttu-id="df399-p107">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="df399-p107">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="df399-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="df399-179">lastModifiedBy</span></span>       | <span data-ttu-id="df399-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="df399-180">[identitySet][]</span></span>   | <span data-ttu-id="df399-181">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="df399-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="df399-182">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="df399-182">Read-only.</span></span>
| <span data-ttu-id="df399-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df399-183">lastModifiedDateTime</span></span> | <span data-ttu-id="df399-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df399-184">DateTimeOffset</span></span>    | <span data-ttu-id="df399-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="df399-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="df399-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="df399-187">parentReference</span></span>      | <span data-ttu-id="df399-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="df399-188">[itemReference][]</span></span> | <span data-ttu-id="df399-p110">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="df399-p110">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="df399-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="df399-191">webUrl</span></span>               | <span data-ttu-id="df399-192">string (URL)</span><span class="sxs-lookup"><span data-stu-id="df399-192">string (url)</span></span>      | <span data-ttu-id="df399-p111">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="df399-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="df399-195">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="df399-195">Relationships</span></span>

<span data-ttu-id="df399-196">**SitePage**リソースには、他のリソースへのリレーションシップがありません。</span><span class="sxs-lookup"><span data-stu-id="df399-196">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[リスト]: list.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
[web パーツ]: webpart.md
[webPart]: webpart.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  }
} -->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
