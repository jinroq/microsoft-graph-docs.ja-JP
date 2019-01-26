---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9ecc23abbee165bce9fd4d9a2a5d8aac8aa02f41
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576242"
---
# <a name="sitepage-resource"></a><span data-ttu-id="528b3-102">sitePage リソース</span><span class="sxs-lookup"><span data-stu-id="528b3-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="528b3-103">このリソースは、サイト ページの[一覧][]でページを表します。</span><span class="sxs-lookup"><span data-stu-id="528b3-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="528b3-104">タイトル、レイアウト、および[web パーツ][]の s のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="528b3-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="528b3-105">ページ上のタスク</span><span class="sxs-lookup"><span data-stu-id="528b3-105">Tasks on a page</span></span>

<span data-ttu-id="528b3-106">**SitePage**リソースの次のタスクを利用できます。</span><span class="sxs-lookup"><span data-stu-id="528b3-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="528b3-107">以下のすべての例は、[サイト][]では、例えば: `https://graph.microsoft.com/{api-version}/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="528b3-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="528b3-108">共通タスク</span><span class="sxs-lookup"><span data-stu-id="528b3-108">Common task</span></span>                     | <span data-ttu-id="528b3-109">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="528b3-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="528b3-110">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="528b3-110">[List pages][]</span></span>                  | <span data-ttu-id="528b3-111">/Pages を取得します。</span><span class="sxs-lookup"><span data-stu-id="528b3-111">GET /pages</span></span>
| <span data-ttu-id="528b3-112">[Get page][]</span><span class="sxs-lookup"><span data-stu-id="528b3-112">[Get page][]</span></span>                    | <span data-ttu-id="528b3-113">/Pages/{ページの id を取得します。</span><span class="sxs-lookup"><span data-stu-id="528b3-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="528b3-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="528b3-114">[Create][]</span></span>                      | <span data-ttu-id="528b3-115">投稿/pages</span><span class="sxs-lookup"><span data-stu-id="528b3-115">POST /pages</span></span>
| <span data-ttu-id="528b3-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="528b3-116">[Delete][]</span></span>                      | <span data-ttu-id="528b3-117">/Pages/{ページの id を削除します。</span><span class="sxs-lookup"><span data-stu-id="528b3-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="528b3-118">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="528b3-118">[Publish][]</span></span>                     | <span data-ttu-id="528b3-119">/Pages/{ページ id} の投稿し、公開</span><span class="sxs-lookup"><span data-stu-id="528b3-119">POST /pages/{page-id}/publish</span></span>

[List pages]: ../api/sitepage-list.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="528b3-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="528b3-125">JSON representation</span></span>

<span data-ttu-id="528b3-126">ここでは、 **sitePage**リソースの JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="528b3-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

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

## <a name="properties"></a><span data-ttu-id="528b3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="528b3-127">Properties</span></span>

<span data-ttu-id="528b3-128">**SitePage**リソースでは、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="528b3-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="528b3-129">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="528b3-129">Property name</span></span>    | <span data-ttu-id="528b3-130">型</span><span class="sxs-lookup"><span data-stu-id="528b3-130">Type</span></span>                         | <span data-ttu-id="528b3-131">説明</span><span class="sxs-lookup"><span data-stu-id="528b3-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="528b3-132">contentType</span><span class="sxs-lookup"><span data-stu-id="528b3-132">contentType</span></span>      | <span data-ttu-id="528b3-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="528b3-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="528b3-134">ページのコンテンツの種類です。</span><span class="sxs-lookup"><span data-stu-id="528b3-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="528b3-135">ページのコンテンツ</span><span class="sxs-lookup"><span data-stu-id="528b3-135">Page Content</span></span>

<span data-ttu-id="528b3-136">**SitePage**リソースでは、次のコンテンツのフィールドがあります。</span><span class="sxs-lookup"><span data-stu-id="528b3-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="528b3-137">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="528b3-137">Property name</span></span>      | <span data-ttu-id="528b3-138">型</span><span class="sxs-lookup"><span data-stu-id="528b3-138">Type</span></span>                       | <span data-ttu-id="528b3-139">説明</span><span class="sxs-lookup"><span data-stu-id="528b3-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="528b3-140">タイトル</span><span class="sxs-lookup"><span data-stu-id="528b3-140">title</span></span>              | <span data-ttu-id="528b3-141">文字列</span><span class="sxs-lookup"><span data-stu-id="528b3-141">string</span></span>                     | <span data-ttu-id="528b3-142">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="528b3-142">The title of the page.</span></span>
| <span data-ttu-id="528b3-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="528b3-143">pageLayout</span></span>         | <span data-ttu-id="528b3-144">文字列</span><span class="sxs-lookup"><span data-stu-id="528b3-144">string</span></span>                     | <span data-ttu-id="528b3-145">ページのページ レイアウトの名前。</span><span class="sxs-lookup"><span data-stu-id="528b3-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="528b3-146">web パーツ</span><span class="sxs-lookup"><span data-stu-id="528b3-146">webParts</span></span>           | <span data-ttu-id="528b3-147">[web パーツ][]</span><span class="sxs-lookup"><span data-stu-id="528b3-147">[webPart][]</span></span>                | <span data-ttu-id="528b3-148">ページ上の web パーツです。</span><span class="sxs-lookup"><span data-stu-id="528b3-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="528b3-149">メタデータを作成する</span><span class="sxs-lookup"><span data-stu-id="528b3-149">Authoring Metadata</span></span>

<span data-ttu-id="528b3-150">**SitePage**のリソースには、次の作成に関連するメタデータがあります。</span><span class="sxs-lookup"><span data-stu-id="528b3-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="528b3-151">PublishingState プロパティは、このようなチェック アウトされているか、公開の状態を作成するページに反映されます。</span><span class="sxs-lookup"><span data-stu-id="528b3-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="528b3-152">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="528b3-152">Property name</span></span>          | <span data-ttu-id="528b3-153">型</span><span class="sxs-lookup"><span data-stu-id="528b3-153">Type</span></span>                   | <span data-ttu-id="528b3-154">説明</span><span class="sxs-lookup"><span data-stu-id="528b3-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="528b3-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="528b3-155">publishingState</span></span>        | <span data-ttu-id="528b3-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="528b3-156">[publicationFacet][]</span></span>   | <span data-ttu-id="528b3-157">発行のステータスと MM.mm バージョンのページです。</span><span class="sxs-lookup"><span data-stu-id="528b3-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="528b3-158">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="528b3-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="528b3-159">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="528b3-159">Property name</span></span>        | <span data-ttu-id="528b3-160">型</span><span class="sxs-lookup"><span data-stu-id="528b3-160">Type</span></span>              | <span data-ttu-id="528b3-161">説明</span><span class="sxs-lookup"><span data-stu-id="528b3-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="528b3-162">id</span><span class="sxs-lookup"><span data-stu-id="528b3-162">id</span></span>                   | <span data-ttu-id="528b3-163">文字列</span><span class="sxs-lookup"><span data-stu-id="528b3-163">string</span></span>            | <span data-ttu-id="528b3-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="528b3-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="528b3-166">name</span><span class="sxs-lookup"><span data-stu-id="528b3-166">name</span></span>                 | <span data-ttu-id="528b3-167">文字列</span><span class="sxs-lookup"><span data-stu-id="528b3-167">string</span></span>            | <span data-ttu-id="528b3-168">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="528b3-168">The name / title of the item.</span></span>
| <span data-ttu-id="528b3-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="528b3-169">createdBy</span></span>            | <span data-ttu-id="528b3-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="528b3-170">[identitySet][]</span></span>   | <span data-ttu-id="528b3-171">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="528b3-171">Identity of the creator of this item.</span></span> <span data-ttu-id="528b3-172">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="528b3-172">Read-only.</span></span>
| <span data-ttu-id="528b3-173">eTag</span><span class="sxs-lookup"><span data-stu-id="528b3-173">eTag</span></span>                 | <span data-ttu-id="528b3-174">文字列</span><span class="sxs-lookup"><span data-stu-id="528b3-174">string</span></span>            | <span data-ttu-id="528b3-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="528b3-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="528b3-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="528b3-177">lastModifiedBy</span></span>       | <span data-ttu-id="528b3-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="528b3-178">[identitySet][]</span></span>   | <span data-ttu-id="528b3-179">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="528b3-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="528b3-180">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="528b3-180">Read-only.</span></span>
| <span data-ttu-id="528b3-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="528b3-181">lastModifiedDateTime</span></span> | <span data-ttu-id="528b3-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="528b3-182">DateTimeOffset</span></span>    | <span data-ttu-id="528b3-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="528b3-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="528b3-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="528b3-185">parentReference</span></span>      | <span data-ttu-id="528b3-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="528b3-186">[itemReference][]</span></span> | <span data-ttu-id="528b3-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="528b3-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="528b3-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="528b3-189">webUrl</span></span>               | <span data-ttu-id="528b3-190">string (URL)</span><span class="sxs-lookup"><span data-stu-id="528b3-190">string (url)</span></span>      | <span data-ttu-id="528b3-p110">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="528b3-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="528b3-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="528b3-193">Relationships</span></span>

<span data-ttu-id="528b3-194">**SitePage**リソースには、他のリソースへのリレーションシップがありません。</span><span class="sxs-lookup"><span data-stu-id="528b3-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
[サイト]: site.md
[site]: site.md
[web パーツ]: webpart.md
[webPart]: webpart.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
