---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
ms.openlocfilehash: ba0c01ce1887a32bd8b671cf511104e9128b5efb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="list-resource"></a><span data-ttu-id="d3007-102">List リソース</span><span class="sxs-lookup"><span data-stu-id="d3007-102">List resource</span></span>

<span data-ttu-id="d3007-103">**list** リソースは [site][] 内のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="d3007-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="d3007-104">このリソースには、テンプレートとフィールドの定義を含め、リストの最上位レベルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d3007-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="d3007-105">リスト上のタスク</span><span class="sxs-lookup"><span data-stu-id="d3007-105">Tasks on a list</span></span>

<span data-ttu-id="d3007-106">list リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3007-106">The following tasks are available for {type} resources.</span></span>
<span data-ttu-id="d3007-107">**注:** このベータ版では、リスト上の移動だけが可能であり、リストの作成や更新はできません。</span><span class="sxs-lookup"><span data-stu-id="d3007-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="d3007-108">ただし、[リスト アイテム]の [listItem] の作成または更新は可能です。</span><span class="sxs-lookup"><span data-stu-id="d3007-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="d3007-109">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}` などのサイトからの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="d3007-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="d3007-110">共通タスク</span><span class="sxs-lookup"><span data-stu-id="d3007-110">Common task</span></span>               | <span data-ttu-id="d3007-111">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="d3007-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="d3007-112">[リストを取得する][]</span><span class="sxs-lookup"><span data-stu-id="d3007-112">[Get list][]</span></span>              | <span data-ttu-id="d3007-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="d3007-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="d3007-114">[リスト アイテムを列挙する][]</span><span class="sxs-lookup"><span data-stu-id="d3007-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="d3007-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="d3007-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="d3007-116">[リスト アイテムを更新する][]</span><span class="sxs-lookup"><span data-stu-id="d3007-116">[Update list item][]</span></span>      | <span data-ttu-id="d3007-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="d3007-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="d3007-118">[リスト アイテムを削除する][]</span><span class="sxs-lookup"><span data-stu-id="d3007-118">[Delete list item][]</span></span>      | <span data-ttu-id="d3007-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="d3007-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="d3007-120">[リスト アイテムを作成する][]</span><span class="sxs-lookup"><span data-stu-id="d3007-120">[Create list item][]</span></span>      | <span data-ttu-id="d3007-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="d3007-121">POST /lists/{list-id}</span></span>

[リストを取得する]: ../api/list_get.md
[リスト アイテムを列挙する]: ../api/listitem_list.md
[リスト アイテムを更新する]: ../api/listItem_update.md
[リスト アイテムを削除する]: ../api/listItem_delete.md
[リスト アイテムを作成する]: ../api/listItem_create.md

## <a name="json-representation"></a><span data-ttu-id="d3007-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3007-127">JSON representation</span></span>

<span data-ttu-id="d3007-128">以下は、**list** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d3007-128">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
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

## <a name="properties"></a><span data-ttu-id="d3007-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3007-129">Properties</span></span>

<span data-ttu-id="d3007-130">**list** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="d3007-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="d3007-131">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="d3007-131">Property name</span></span>    | <span data-ttu-id="d3007-132">種類</span><span class="sxs-lookup"><span data-stu-id="d3007-132">Type</span></span>                             | <span data-ttu-id="d3007-133">説明</span><span class="sxs-lookup"><span data-stu-id="d3007-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="d3007-134">**columns**</span><span class="sxs-lookup"><span data-stu-id="d3007-134">**columns**</span></span>      | <span data-ttu-id="d3007-135">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="d3007-135">Collection([columnDefinition][])</span></span> | <span data-ttu-id="d3007-136">このリストのフィールド定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d3007-136">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="d3007-137">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="d3007-137"><ContentTypes></span></span> | <span data-ttu-id="d3007-138">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="d3007-138">Collection([contentType][])</span></span>      | <span data-ttu-id="d3007-139">このリスト内に存在するコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d3007-139">The collection of content types present in this list.</span></span>
| <span data-ttu-id="d3007-140">**displayName**</span><span class="sxs-lookup"><span data-stu-id="d3007-140">**displayName**</span></span>  | <span data-ttu-id="d3007-141">string</span><span class="sxs-lookup"><span data-stu-id="d3007-141">string</span></span>                           | <span data-ttu-id="d3007-142">リストの表示可能なタイトルです。</span><span class="sxs-lookup"><span data-stu-id="d3007-142">The previous title of the list.</span></span>
| <span data-ttu-id="d3007-143">**list**</span><span class="sxs-lookup"><span data-stu-id="d3007-143">**list**</span></span>         | <span data-ttu-id="d3007-144">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="d3007-144">[listInfo][]</span></span>                     | <span data-ttu-id="d3007-145">リストに関する追加の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="d3007-145">Provides additional details about the list.</span></span>
| <span data-ttu-id="d3007-146">**system**</span><span class="sxs-lookup"><span data-stu-id="d3007-146">**System**</span></span>       | <span data-ttu-id="d3007-147">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="d3007-147">[systemFacet][]</span></span>                  | <span data-ttu-id="d3007-148">存在する場合は、これがシステム管理のリストであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="d3007-148">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="d3007-149">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3007-149">Read-only.</span></span>

<span data-ttu-id="d3007-150">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="d3007-150">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="d3007-151">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="d3007-151">Property name</span></span>            | <span data-ttu-id="d3007-152">種類</span><span class="sxs-lookup"><span data-stu-id="d3007-152">Type</span></span>             | <span data-ttu-id="d3007-153">説明</span><span class="sxs-lookup"><span data-stu-id="d3007-153">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="d3007-154">**id**</span><span class="sxs-lookup"><span data-stu-id="d3007-154">**id**</span></span>                   | <span data-ttu-id="d3007-155">string</span><span class="sxs-lookup"><span data-stu-id="d3007-155">string</span></span>           | <span data-ttu-id="d3007-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3007-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="d3007-158">**name**</span><span class="sxs-lookup"><span data-stu-id="d3007-158">**name**</span></span>                 | <span data-ttu-id="d3007-159">string</span><span class="sxs-lookup"><span data-stu-id="d3007-159">string</span></span>           | <span data-ttu-id="d3007-160">アイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="d3007-160">The name of the item.</span></span>
| <span data-ttu-id="d3007-161">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="d3007-161">**createdBy**</span></span>            | <span data-ttu-id="d3007-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d3007-162">[identitySet][]</span></span>  | <span data-ttu-id="d3007-163">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="d3007-163">Identity of the creator of this item.</span></span> <span data-ttu-id="d3007-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3007-164">Read-only.</span></span>
| <span data-ttu-id="d3007-165">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="d3007-165">**createdDateTime**</span></span>      | <span data-ttu-id="d3007-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3007-166">DateTimeOffset</span></span>   | <span data-ttu-id="d3007-p106">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3007-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="d3007-169">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3007-169">**description**</span></span>          | <span data-ttu-id="d3007-170">string</span><span class="sxs-lookup"><span data-stu-id="d3007-170">string</span></span>           | <span data-ttu-id="d3007-171">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="d3007-171">The descriptive text for the site.</span></span>
| <span data-ttu-id="d3007-172">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="d3007-172">**lastModifiedBy**</span></span>       | <span data-ttu-id="d3007-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d3007-173">[identitySet][]</span></span>  | <span data-ttu-id="d3007-174">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="d3007-174">Identity of the last modifier of this item.</span></span> <span data-ttu-id="d3007-175">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3007-175">Read-only.</span></span>
| <span data-ttu-id="d3007-176">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d3007-176">**lastModifiedDateTime**</span></span> | <span data-ttu-id="d3007-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3007-177">DateTimeOffset</span></span>   | <span data-ttu-id="d3007-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3007-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="d3007-180">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="d3007-180">**webUrl**</span></span>               | <span data-ttu-id="d3007-181">string (URL)</span><span class="sxs-lookup"><span data-stu-id="d3007-181">string (url)</span></span>     | <span data-ttu-id="d3007-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3007-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="d3007-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3007-184">Relationships</span></span>

<span data-ttu-id="d3007-185">**list** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="d3007-185">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="d3007-186">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="d3007-186">Relationship name</span></span> | <span data-ttu-id="d3007-187">種類</span><span class="sxs-lookup"><span data-stu-id="d3007-187">Type</span></span>                        | <span data-ttu-id="d3007-188">説明</span><span class="sxs-lookup"><span data-stu-id="d3007-188">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="d3007-189">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="d3007-189">**drive**</span></span>         | <span data-ttu-id="d3007-190">[drive][]</span><span class="sxs-lookup"><span data-stu-id="d3007-190">[drive][]</span></span>                   | <span data-ttu-id="d3007-191">ドキュメント ライブラリにのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="d3007-191">Only present on document libraries.</span></span> <span data-ttu-id="d3007-192">[driveItems][driveItem] を含む [drive][] リソースとしてリストにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d3007-192">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="d3007-193">**items**</span><span class="sxs-lookup"><span data-stu-id="d3007-193">**items**</span></span>         | <span data-ttu-id="d3007-194">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="d3007-194">Collection([listItem][])</span></span>    | <span data-ttu-id="d3007-195">リストに含まれているすべてのアイテム。</span><span class="sxs-lookup"><span data-stu-id="d3007-195">All items contained in the drive.</span></span>

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[listInfo]: listInfo.md
[listItem]: listItem.md
[site]: site.md
[systemFacet]: systemFacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  }
} -->
