---
author: JeremyKelley
description: list リソースは site 内のリストを表します。
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b79172049278758c77ac620f00c391d52633792b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009994"
---
# <a name="list-resource"></a><span data-ttu-id="a6d2b-103">List リソース</span><span class="sxs-lookup"><span data-stu-id="a6d2b-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6d2b-104">**list** リソースは [site][] 内のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="a6d2b-105">このリソースには、テンプレートとフィールドの定義を含め、リストの最上位レベルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="a6d2b-106">リスト上のタスク</span><span class="sxs-lookup"><span data-stu-id="a6d2b-106">Tasks on a list</span></span>

<span data-ttu-id="a6d2b-107">list リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="a6d2b-108">**注:** このベータ版では、リスト上の移動だけが可能であり、リストの作成や更新はできません。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="a6d2b-109">ただし、[リスト アイテム]の [listItem] の作成または更新は可能です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="a6d2b-110">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}` などのサイトからの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="a6d2b-111">共通タスク</span><span class="sxs-lookup"><span data-stu-id="a6d2b-111">Common task</span></span>               | <span data-ttu-id="a6d2b-112">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="a6d2b-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="a6d2b-113">[リストを取得する][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-113">[Get list][]</span></span>              | <span data-ttu-id="a6d2b-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="a6d2b-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="a6d2b-115">[リスト アイテムを列挙する][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-115">[Enumerate list items][]</span></span>  | <span data-ttu-id="a6d2b-116">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="a6d2b-116">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="a6d2b-117">[リスト アイテムを更新する][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-117">[Update list item][]</span></span>      | <span data-ttu-id="a6d2b-118">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a6d2b-118">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="a6d2b-119">[リスト アイテムを削除する][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-119">[Delete list item][]</span></span>      | <span data-ttu-id="a6d2b-120">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a6d2b-120">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="a6d2b-121">[リスト アイテムを作成する][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-121">[Create list item][]</span></span>      | <span data-ttu-id="a6d2b-122">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="a6d2b-122">POST /lists/{list-id}</span></span>
| <span data-ttu-id="a6d2b-123">[最近のアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-123">[Get recent activities][]</span></span> | <span data-ttu-id="a6d2b-124">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="a6d2b-124">GET /lists/{list-id}/activities</span></span>

[リストを取得する]: ../api/list-get.md
[Get list]: ../api/list-get.md
[リスト アイテムを列挙する]: ../api/listitem-list.md
[Enumerate list items]: ../api/listitem-list.md
[リスト アイテムを更新する]: ../api/listitem-update.md
[Update list item]: ../api/listitem-update.md
[リスト アイテムを削除する]: ../api/listitem-delete.md
[Delete list item]: ../api/listitem-delete.md
[リスト アイテムを作成する]: ../api/listitem-create.md
[Create list item]: ../api/listitem-create.md
[最近のアクティビティを取得する]: ../api/activities-list.md
[Get recent activities]: ../api/activities-list.md

## <a name="json-representation"></a><span data-ttu-id="a6d2b-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6d2b-131">JSON representation</span></span>

<span data-ttu-id="a6d2b-132">以下は、**list** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-132">Here is a JSON representation of a **list** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
  },
  "system": false,

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="a6d2b-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6d2b-133">Properties</span></span>

<span data-ttu-id="a6d2b-134">**list** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-134">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="a6d2b-135">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a6d2b-135">Property name</span></span>    | <span data-ttu-id="a6d2b-136">種類</span><span class="sxs-lookup"><span data-stu-id="a6d2b-136">Type</span></span>                             | <span data-ttu-id="a6d2b-137">説明</span><span class="sxs-lookup"><span data-stu-id="a6d2b-137">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="a6d2b-138">**columns**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-138">**columns**</span></span>      | <span data-ttu-id="a6d2b-139">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="a6d2b-139">Collection([columnDefinition][])</span></span> | <span data-ttu-id="a6d2b-140">このリストのフィールド定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-140">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="a6d2b-141">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-141">**contentTypes**</span></span> | <span data-ttu-id="a6d2b-142">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="a6d2b-142">Collection([contentType][])</span></span>      | <span data-ttu-id="a6d2b-143">このリスト内に存在するコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-143">The collection of content types present in this list.</span></span>
| <span data-ttu-id="a6d2b-144">**displayName**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-144">**displayName**</span></span>  | <span data-ttu-id="a6d2b-145">string</span><span class="sxs-lookup"><span data-stu-id="a6d2b-145">string</span></span>                           | <span data-ttu-id="a6d2b-146">リストの表示可能なタイトルです。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-146">The displayable title of the list.</span></span>
| <span data-ttu-id="a6d2b-147">**list**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-147">**list**</span></span>         | <span data-ttu-id="a6d2b-148">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-148">[listInfo][]</span></span>                     | <span data-ttu-id="a6d2b-149">リストに関する追加の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-149">Provides additional details about the list.</span></span>
| <span data-ttu-id="a6d2b-150">**system**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-150">**system**</span></span>       | <span data-ttu-id="a6d2b-151">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-151">[systemFacet][]</span></span>                  | <span data-ttu-id="a6d2b-152">存在する場合は、これがシステム管理のリストであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-152">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="a6d2b-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-153">Read-only.</span></span>

<span data-ttu-id="a6d2b-154">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-154">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="a6d2b-155">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a6d2b-155">Property name</span></span>            | <span data-ttu-id="a6d2b-156">種類</span><span class="sxs-lookup"><span data-stu-id="a6d2b-156">Type</span></span>             | <span data-ttu-id="a6d2b-157">説明</span><span class="sxs-lookup"><span data-stu-id="a6d2b-157">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="a6d2b-158">**id**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-158">**id**</span></span>                   | <span data-ttu-id="a6d2b-159">string</span><span class="sxs-lookup"><span data-stu-id="a6d2b-159">string</span></span>           | <span data-ttu-id="a6d2b-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="a6d2b-162">**name**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-162">**name**</span></span>                 | <span data-ttu-id="a6d2b-163">string</span><span class="sxs-lookup"><span data-stu-id="a6d2b-163">string</span></span>           | <span data-ttu-id="a6d2b-164">アイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-164">The name of the item.</span></span>
| <span data-ttu-id="a6d2b-165">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-165">**createdBy**</span></span>            | <span data-ttu-id="a6d2b-166">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-166">[identitySet][]</span></span>  | <span data-ttu-id="a6d2b-167">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-167">Identity of the creator of this item.</span></span> <span data-ttu-id="a6d2b-168">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-168">Read-only.</span></span>
| <span data-ttu-id="a6d2b-169">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-169">**createdDateTime**</span></span>      | <span data-ttu-id="a6d2b-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6d2b-170">DateTimeOffset</span></span>   | <span data-ttu-id="a6d2b-p106">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="a6d2b-173">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-173">**description**</span></span>          | <span data-ttu-id="a6d2b-174">string</span><span class="sxs-lookup"><span data-stu-id="a6d2b-174">string</span></span>           | <span data-ttu-id="a6d2b-175">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-175">The descriptive text for the item.</span></span>
| <span data-ttu-id="a6d2b-176">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-176">**lastModifiedBy**</span></span>       | <span data-ttu-id="a6d2b-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-177">[identitySet][]</span></span>  | <span data-ttu-id="a6d2b-178">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-178">Identity of the last modifier of this item.</span></span> <span data-ttu-id="a6d2b-179">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-179">Read-only.</span></span>
| <span data-ttu-id="a6d2b-180">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-180">**lastModifiedDateTime**</span></span> | <span data-ttu-id="a6d2b-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6d2b-181">DateTimeOffset</span></span>   | <span data-ttu-id="a6d2b-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="a6d2b-184">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-184">**webUrl**</span></span>               | <span data-ttu-id="a6d2b-185">string (URL)</span><span class="sxs-lookup"><span data-stu-id="a6d2b-185">string (url)</span></span>     | <span data-ttu-id="a6d2b-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="a6d2b-188">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6d2b-188">Relationships</span></span>

<span data-ttu-id="a6d2b-189">**list** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-189">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="a6d2b-190">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="a6d2b-190">Relationship name</span></span> | <span data-ttu-id="a6d2b-191">種類</span><span class="sxs-lookup"><span data-stu-id="a6d2b-191">Type</span></span>                        | <span data-ttu-id="a6d2b-192">説明</span><span class="sxs-lookup"><span data-stu-id="a6d2b-192">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="a6d2b-193">**activities**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-193">**activities**</span></span>    | <span data-ttu-id="a6d2b-194">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="a6d2b-194">[itemActivity][] collection</span></span> | <span data-ttu-id="a6d2b-195">このリスト内で行われた最近のアクティビティです。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-195">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="a6d2b-196">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-196">**drive**</span></span>         | <span data-ttu-id="a6d2b-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="a6d2b-197">[drive][]</span></span>                   | <span data-ttu-id="a6d2b-198">ドキュメント ライブラリにのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-198">Only present on document libraries.</span></span> <span data-ttu-id="a6d2b-199">[driveItems][driveItem] を含む [drive][] リソースとしてリストにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-199">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="a6d2b-200">**items**</span><span class="sxs-lookup"><span data-stu-id="a6d2b-200">**items**</span></span>         | <span data-ttu-id="a6d2b-201">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="a6d2b-201">Collection([listItem][])</span></span>    | <span data-ttu-id="a6d2b-202">リストに含まれているすべてのアイテム。</span><span class="sxs-lookup"><span data-stu-id="a6d2b-202">All items contained in the list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[サイト]: site.md
[site]: site.md
[systemFacet]: systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  },
  "suppressions": []
}
-->
