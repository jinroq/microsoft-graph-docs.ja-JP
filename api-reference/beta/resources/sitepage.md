---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: sitepage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6a9192423c4caf47913029e3671e975884533333
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343079"
---
# <a name="sitepage-resource"></a><span data-ttu-id="630d6-102">sitepage リソース</span><span class="sxs-lookup"><span data-stu-id="630d6-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="630d6-103">このリソースは、sitepages[リスト][]のページを表します。</span><span class="sxs-lookup"><span data-stu-id="630d6-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="630d6-104">これには、タイトル、レイアウト、および[webPart][]のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="630d6-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="630d6-105">ページ上のタスク</span><span class="sxs-lookup"><span data-stu-id="630d6-105">Tasks on a page</span></span>

<span data-ttu-id="630d6-106">**sitepage**リソースでは、次のタスクを使用できます。</span><span class="sxs-lookup"><span data-stu-id="630d6-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="630d6-107">以下のすべての例は、[サイト][]に関連し`https://graph.microsoft.com/{api-version}/sites/{site-id}`ています。例:。</span><span class="sxs-lookup"><span data-stu-id="630d6-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="630d6-108">共通タスク</span><span class="sxs-lookup"><span data-stu-id="630d6-108">Common task</span></span>                     | <span data-ttu-id="630d6-109">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="630d6-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="630d6-110">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="630d6-110">[List pages][]</span></span>                  | <span data-ttu-id="630d6-111">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="630d6-111">GET /pages</span></span>
| <span data-ttu-id="630d6-112">[ページを取得する][]</span><span class="sxs-lookup"><span data-stu-id="630d6-112">[Get page][]</span></span>                    | <span data-ttu-id="630d6-113">ページを取得する/ページ/{pagefrom id}</span><span class="sxs-lookup"><span data-stu-id="630d6-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="630d6-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="630d6-114">[Create][]</span></span>                      | <span data-ttu-id="630d6-115">投稿/ページ</span><span class="sxs-lookup"><span data-stu-id="630d6-115">POST /pages</span></span>
| <span data-ttu-id="630d6-116">[削除][]</span><span class="sxs-lookup"><span data-stu-id="630d6-116">[Delete][]</span></span>                      | <span data-ttu-id="630d6-117">削除/ページ/{page¥ id}</span><span class="sxs-lookup"><span data-stu-id="630d6-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="630d6-118">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="630d6-118">[Publish][]</span></span>                     | <span data-ttu-id="630d6-119">投稿/ページ/_ page/発行</span><span class="sxs-lookup"><span data-stu-id="630d6-119">POST /pages/{page-id}/publish</span></span>

[List pages]: ../api/sitepage-list.md
[ページを取得する]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="630d6-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="630d6-125">JSON representation</span></span>

<span data-ttu-id="630d6-126">ここでは、 **sitepage**リソースの JSON 表記を示します。</span><span class="sxs-lookup"><span data-stu-id="630d6-126">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage",
  "openType": true
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayoutType": "String",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

   /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="630d6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="630d6-127">Properties</span></span>

<span data-ttu-id="630d6-128">**sitepage**リソースには、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="630d6-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="630d6-129">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="630d6-129">Property name</span></span>    | <span data-ttu-id="630d6-130">種類</span><span class="sxs-lookup"><span data-stu-id="630d6-130">Type</span></span>                         | <span data-ttu-id="630d6-131">説明</span><span class="sxs-lookup"><span data-stu-id="630d6-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="630d6-132">contentType</span><span class="sxs-lookup"><span data-stu-id="630d6-132">contentType</span></span>      | <span data-ttu-id="630d6-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="630d6-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="630d6-134">ページのコンテンツタイプ。</span><span class="sxs-lookup"><span data-stu-id="630d6-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="630d6-135">ページのコンテンツ</span><span class="sxs-lookup"><span data-stu-id="630d6-135">Page Content</span></span>

<span data-ttu-id="630d6-136">**sitepage**リソースには、次のコンテンツフィールドがあります。</span><span class="sxs-lookup"><span data-stu-id="630d6-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="630d6-137">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="630d6-137">Property name</span></span>      | <span data-ttu-id="630d6-138">種類</span><span class="sxs-lookup"><span data-stu-id="630d6-138">Type</span></span>                       | <span data-ttu-id="630d6-139">説明</span><span class="sxs-lookup"><span data-stu-id="630d6-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="630d6-140">title</span><span class="sxs-lookup"><span data-stu-id="630d6-140">title</span></span>              | <span data-ttu-id="630d6-141">string</span><span class="sxs-lookup"><span data-stu-id="630d6-141">string</span></span>                     | <span data-ttu-id="630d6-142">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="630d6-142">The title of the page.</span></span>
| <span data-ttu-id="630d6-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="630d6-143">pageLayout</span></span>         | <span data-ttu-id="630d6-144">string</span><span class="sxs-lookup"><span data-stu-id="630d6-144">string</span></span>                     | <span data-ttu-id="630d6-145">ページのページレイアウトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="630d6-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="630d6-146">パーツ</span><span class="sxs-lookup"><span data-stu-id="630d6-146">webParts</span></span>           | <span data-ttu-id="630d6-147">[パーツ][]</span><span class="sxs-lookup"><span data-stu-id="630d6-147">[webPart][]</span></span>                | <span data-ttu-id="630d6-148">ページ上の web パーツ。</span><span class="sxs-lookup"><span data-stu-id="630d6-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="630d6-149">メタデータを作成する</span><span class="sxs-lookup"><span data-stu-id="630d6-149">Authoring Metadata</span></span>

<span data-ttu-id="630d6-150">**sitepage**リソースには、次の作成関連のメタデータがあります。</span><span class="sxs-lookup"><span data-stu-id="630d6-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="630d6-151">発行状態プロパティは、チェックアウトまたは発行されたページ作成状態を反映します。</span><span class="sxs-lookup"><span data-stu-id="630d6-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="630d6-152">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="630d6-152">Property name</span></span>          | <span data-ttu-id="630d6-153">種類</span><span class="sxs-lookup"><span data-stu-id="630d6-153">Type</span></span>                   | <span data-ttu-id="630d6-154">説明</span><span class="sxs-lookup"><span data-stu-id="630d6-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="630d6-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="630d6-155">publishingState</span></span>        | <span data-ttu-id="630d6-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="630d6-156">[publicationFacet][]</span></span>   | <span data-ttu-id="630d6-157">ページの発行状態と MM.mm バージョン。</span><span class="sxs-lookup"><span data-stu-id="630d6-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="630d6-158">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="630d6-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="630d6-159">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="630d6-159">Property name</span></span>        | <span data-ttu-id="630d6-160">種類</span><span class="sxs-lookup"><span data-stu-id="630d6-160">Type</span></span>              | <span data-ttu-id="630d6-161">説明</span><span class="sxs-lookup"><span data-stu-id="630d6-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="630d6-162">id</span><span class="sxs-lookup"><span data-stu-id="630d6-162">id</span></span>                   | <span data-ttu-id="630d6-163">string</span><span class="sxs-lookup"><span data-stu-id="630d6-163">string</span></span>            | <span data-ttu-id="630d6-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="630d6-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="630d6-166">name</span><span class="sxs-lookup"><span data-stu-id="630d6-166">name</span></span>                 | <span data-ttu-id="630d6-167">string</span><span class="sxs-lookup"><span data-stu-id="630d6-167">string</span></span>            | <span data-ttu-id="630d6-168">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="630d6-168">The name / title of the item.</span></span>
| <span data-ttu-id="630d6-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="630d6-169">createdBy</span></span>            | <span data-ttu-id="630d6-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="630d6-170">[identitySet][]</span></span>   | <span data-ttu-id="630d6-171">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="630d6-171">Identity of the creator of this item.</span></span> <span data-ttu-id="630d6-172">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="630d6-172">Read-only.</span></span>
| <span data-ttu-id="630d6-173">eTag</span><span class="sxs-lookup"><span data-stu-id="630d6-173">eTag</span></span>                 | <span data-ttu-id="630d6-174">string</span><span class="sxs-lookup"><span data-stu-id="630d6-174">string</span></span>            | <span data-ttu-id="630d6-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="630d6-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="630d6-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="630d6-177">lastModifiedBy</span></span>       | <span data-ttu-id="630d6-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="630d6-178">[identitySet][]</span></span>   | <span data-ttu-id="630d6-179">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="630d6-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="630d6-180">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="630d6-180">Read-only.</span></span>
| <span data-ttu-id="630d6-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="630d6-181">lastModifiedDateTime</span></span> | <span data-ttu-id="630d6-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="630d6-182">DateTimeOffset</span></span>    | <span data-ttu-id="630d6-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="630d6-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="630d6-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="630d6-185">parentReference</span></span>      | <span data-ttu-id="630d6-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="630d6-186">[itemReference][]</span></span> | <span data-ttu-id="630d6-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="630d6-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="630d6-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="630d6-189">webUrl</span></span>               | <span data-ttu-id="630d6-190">string (URL)</span><span class="sxs-lookup"><span data-stu-id="630d6-190">string (url)</span></span>      | <span data-ttu-id="630d6-p110">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="630d6-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="630d6-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="630d6-193">Relationships</span></span>

<span data-ttu-id="630d6-194">**sitepage**リソースには、他のリソースとの関係がありません。</span><span class="sxs-lookup"><span data-stu-id="630d6-194">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[サイト]: site.md
[site]: site.md
[パーツ]: webpart.md
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
  "suppressions": []
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
