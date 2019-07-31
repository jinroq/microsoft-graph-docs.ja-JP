---
author: rahmit
description: このリソースは、SitePages リストのページを表します。
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 240ab50f31d500fad960768bb6c45cb9c6ff6511
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965048"
---
# <a name="sitepage-resource"></a><span data-ttu-id="2e8d5-103">sitePage リソース</span><span class="sxs-lookup"><span data-stu-id="2e8d5-103">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e8d5-104">このリソースは、SitePages[リスト][]のページを表します。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-104">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="2e8d5-105">これには、タイトル、レイアウト、および[webPart][]のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-105">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="2e8d5-106">ページ上のタスク</span><span class="sxs-lookup"><span data-stu-id="2e8d5-106">Tasks on a page</span></span>

<span data-ttu-id="2e8d5-107">**Sitepage**リソースでは、次のタスクを使用できます。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-107">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="2e8d5-108">以下のすべての例は、[サイト][]に関連し`https://graph.microsoft.com/{api-version}/sites/{site-id}`ています。例:。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-108">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="2e8d5-109">共通タスク</span><span class="sxs-lookup"><span data-stu-id="2e8d5-109">Common task</span></span>                     | <span data-ttu-id="2e8d5-110">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="2e8d5-110">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="2e8d5-111">[ページを一覧表示する][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-111">[List pages][]</span></span>                  | <span data-ttu-id="2e8d5-112">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="2e8d5-112">GET /pages</span></span>
| <span data-ttu-id="2e8d5-113">[ページを取得する][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-113">[Get page][]</span></span>                    | <span data-ttu-id="2e8d5-114">ページを取得する/ページ/{pagefrom id}</span><span class="sxs-lookup"><span data-stu-id="2e8d5-114">GET /pages/{page-id}</span></span>
| <span data-ttu-id="2e8d5-115">[Create][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-115">[Create][]</span></span>                      | <span data-ttu-id="2e8d5-116">投稿/ページ</span><span class="sxs-lookup"><span data-stu-id="2e8d5-116">POST /pages</span></span>
| <span data-ttu-id="2e8d5-117">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-117">[Delete][]</span></span>                      | <span data-ttu-id="2e8d5-118">削除/ページ/{page¥ id}</span><span class="sxs-lookup"><span data-stu-id="2e8d5-118">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="2e8d5-119">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-119">[Publish][]</span></span>                     | <span data-ttu-id="2e8d5-120">投稿/ページ/_ page/発行</span><span class="sxs-lookup"><span data-stu-id="2e8d5-120">POST /pages/{page-id}/publish</span></span>

[ページを一覧表示する]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[ページを取得する]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="2e8d5-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e8d5-126">JSON representation</span></span>

<span data-ttu-id="2e8d5-127">ここでは、 **Sitepage**リソースの JSON 表記を示します。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-127">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2e8d5-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e8d5-128">Properties</span></span>

<span data-ttu-id="2e8d5-129">**Sitepage**リソースには、次のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-129">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="2e8d5-130">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2e8d5-130">Property name</span></span>    | <span data-ttu-id="2e8d5-131">種類</span><span class="sxs-lookup"><span data-stu-id="2e8d5-131">Type</span></span>                         | <span data-ttu-id="2e8d5-132">説明</span><span class="sxs-lookup"><span data-stu-id="2e8d5-132">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="2e8d5-133">contentType</span><span class="sxs-lookup"><span data-stu-id="2e8d5-133">contentType</span></span>      | <span data-ttu-id="2e8d5-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-134">[contentTypeInfo][]</span></span>          | <span data-ttu-id="2e8d5-135">ページのコンテンツタイプ。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-135">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="2e8d5-136">ページのコンテンツ</span><span class="sxs-lookup"><span data-stu-id="2e8d5-136">Page Content</span></span>

<span data-ttu-id="2e8d5-137">**Sitepage**リソースには、次のコンテンツフィールドがあります。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-137">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="2e8d5-138">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2e8d5-138">Property name</span></span>      | <span data-ttu-id="2e8d5-139">種類</span><span class="sxs-lookup"><span data-stu-id="2e8d5-139">Type</span></span>                       | <span data-ttu-id="2e8d5-140">説明</span><span class="sxs-lookup"><span data-stu-id="2e8d5-140">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="2e8d5-141">title</span><span class="sxs-lookup"><span data-stu-id="2e8d5-141">title</span></span>              | <span data-ttu-id="2e8d5-142">string</span><span class="sxs-lookup"><span data-stu-id="2e8d5-142">string</span></span>                     | <span data-ttu-id="2e8d5-143">ページのタイトル。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-143">The title of the page.</span></span>
| <span data-ttu-id="2e8d5-144">pageLayout</span><span class="sxs-lookup"><span data-stu-id="2e8d5-144">pageLayout</span></span>         | <span data-ttu-id="2e8d5-145">string</span><span class="sxs-lookup"><span data-stu-id="2e8d5-145">string</span></span>                     | <span data-ttu-id="2e8d5-146">ページのページレイアウトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-146">The name of the page layout of the page.</span></span>
| <span data-ttu-id="2e8d5-147">パーツ</span><span class="sxs-lookup"><span data-stu-id="2e8d5-147">webParts</span></span>           | <span data-ttu-id="2e8d5-148">[パーツ][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-148">[webPart][]</span></span>                | <span data-ttu-id="2e8d5-149">ページ上の web パーツ。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-149">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="2e8d5-150">メタデータを作成する</span><span class="sxs-lookup"><span data-stu-id="2e8d5-150">Authoring Metadata</span></span>

<span data-ttu-id="2e8d5-151">**Sitepage**リソースには、次の作成関連のメタデータがあります。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-151">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="2e8d5-152">発行状態プロパティは、チェックアウトまたは発行されたページ作成状態を反映します。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-152">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="2e8d5-153">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2e8d5-153">Property name</span></span>          | <span data-ttu-id="2e8d5-154">種類</span><span class="sxs-lookup"><span data-stu-id="2e8d5-154">Type</span></span>                   | <span data-ttu-id="2e8d5-155">説明</span><span class="sxs-lookup"><span data-stu-id="2e8d5-155">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="2e8d5-156">publishingState</span><span class="sxs-lookup"><span data-stu-id="2e8d5-156">publishingState</span></span>        | <span data-ttu-id="2e8d5-157">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-157">[publicationFacet][]</span></span>   | <span data-ttu-id="2e8d5-158">ページの発行状態と MM.mm バージョン。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-158">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="2e8d5-159">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-159">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="2e8d5-160">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2e8d5-160">Property name</span></span>        | <span data-ttu-id="2e8d5-161">種類</span><span class="sxs-lookup"><span data-stu-id="2e8d5-161">Type</span></span>              | <span data-ttu-id="2e8d5-162">説明</span><span class="sxs-lookup"><span data-stu-id="2e8d5-162">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="2e8d5-163">id</span><span class="sxs-lookup"><span data-stu-id="2e8d5-163">id</span></span>                   | <span data-ttu-id="2e8d5-164">string</span><span class="sxs-lookup"><span data-stu-id="2e8d5-164">string</span></span>            | <span data-ttu-id="2e8d5-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="2e8d5-167">name</span><span class="sxs-lookup"><span data-stu-id="2e8d5-167">name</span></span>                 | <span data-ttu-id="2e8d5-168">string</span><span class="sxs-lookup"><span data-stu-id="2e8d5-168">string</span></span>            | <span data-ttu-id="2e8d5-169">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-169">The name / title of the item.</span></span>
| <span data-ttu-id="2e8d5-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="2e8d5-170">createdBy</span></span>            | <span data-ttu-id="2e8d5-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-171">[identitySet][]</span></span>   | <span data-ttu-id="2e8d5-172">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-172">Identity of the creator of this item.</span></span> <span data-ttu-id="2e8d5-173">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-173">Read-only.</span></span>
| <span data-ttu-id="2e8d5-174">eTag</span><span class="sxs-lookup"><span data-stu-id="2e8d5-174">eTag</span></span>                 | <span data-ttu-id="2e8d5-175">string</span><span class="sxs-lookup"><span data-stu-id="2e8d5-175">string</span></span>            | <span data-ttu-id="2e8d5-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="2e8d5-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2e8d5-178">lastModifiedBy</span></span>       | <span data-ttu-id="2e8d5-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-179">[identitySet][]</span></span>   | <span data-ttu-id="2e8d5-180">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="2e8d5-181">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-181">Read-only.</span></span>
| <span data-ttu-id="2e8d5-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e8d5-182">lastModifiedDateTime</span></span> | <span data-ttu-id="2e8d5-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e8d5-183">DateTimeOffset</span></span>    | <span data-ttu-id="2e8d5-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="2e8d5-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="2e8d5-186">parentReference</span></span>      | <span data-ttu-id="2e8d5-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="2e8d5-187">[itemReference][]</span></span> | <span data-ttu-id="2e8d5-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="2e8d5-190">webUrl</span><span class="sxs-lookup"><span data-stu-id="2e8d5-190">webUrl</span></span>               | <span data-ttu-id="2e8d5-191">string (URL)</span><span class="sxs-lookup"><span data-stu-id="2e8d5-191">string (url)</span></span>      | <span data-ttu-id="2e8d5-p110">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="2e8d5-194">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e8d5-194">Relationships</span></span>

<span data-ttu-id="2e8d5-195">**Sitepage**リソースには、他のリソースとの関係がありません。</span><span class="sxs-lookup"><span data-stu-id="2e8d5-195">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[リスト]: site.md
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
