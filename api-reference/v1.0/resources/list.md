---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 6bfd46e0822045869074cb0d78f14e3f0be0c994
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984389"
---
# <a name="list-resource"></a><span data-ttu-id="a5a4a-102">list リソース</span><span class="sxs-lookup"><span data-stu-id="a5a4a-102">List resource</span></span>

<span data-ttu-id="a5a4a-103">**list** リソースは [site][] 内のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="a5a4a-104">このリソースには、テンプレートとフィールドの定義を含め、リストの最上位レベルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="a5a4a-105">リスト上のタスク</span><span class="sxs-lookup"><span data-stu-id="a5a4a-105">Tasks on a list</span></span>

<span data-ttu-id="a5a4a-106">list リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="a5a4a-107">**注:** このベータ版では、リスト上の移動だけが可能であり、リストの作成や更新はできません。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="a5a4a-108">ただし、[リスト アイテム]の [listItem] の作成または更新は可能です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="a5a4a-109">以下のすべての例は、`https://graph.microsoft.com/v1.0/sites/{site-id}` などのサイトからの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="a5a4a-110">共通タスク</span><span class="sxs-lookup"><span data-stu-id="a5a4a-110">Common task</span></span>               | <span data-ttu-id="a5a4a-111">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="a5a4a-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="a5a4a-112">[リストを取得する][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-112">[Get list][]</span></span>              | <span data-ttu-id="a5a4a-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="a5a4a-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="a5a4a-114">[リスト アイテムを列挙する][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="a5a4a-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="a5a4a-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="a5a4a-116">[リスト アイテムを更新する][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-116">[Update list item][]</span></span>      | <span data-ttu-id="a5a4a-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a5a4a-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="a5a4a-118">[リスト アイテムを削除する][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-118">[Delete list item][]</span></span>      | <span data-ttu-id="a5a4a-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a5a4a-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="a5a4a-120">[リスト アイテムを作成する][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-120">[Create list item][]</span></span>      | <span data-ttu-id="a5a4a-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="a5a4a-121">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="a5a4a-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a5a4a-127">JSON representation</span></span>

<span data-ttu-id="a5a4a-128">以下は、**list** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-128">Here is a JSON representation of a **list** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.list"
}-->

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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
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
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="a5a4a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5a4a-129">Properties</span></span>

<span data-ttu-id="a5a4a-130">**list** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="a5a4a-131">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a5a4a-131">Property name</span></span>    | <span data-ttu-id="a5a4a-132">Type</span><span class="sxs-lookup"><span data-stu-id="a5a4a-132">Type</span></span>                             | <span data-ttu-id="a5a4a-133">説明</span><span class="sxs-lookup"><span data-stu-id="a5a4a-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="a5a4a-134">**displayName**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-134">**displayName**</span></span>  | <span data-ttu-id="a5a4a-135">文字列</span><span class="sxs-lookup"><span data-stu-id="a5a4a-135">string</span></span>                           | <span data-ttu-id="a5a4a-136">リストの表示可能なタイトルです。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-136">The displayable title of the list.</span></span>
| <span data-ttu-id="a5a4a-137">**list**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-137">**list**</span></span>         | <span data-ttu-id="a5a4a-138">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-138">[listInfo][]</span></span>                     | <span data-ttu-id="a5a4a-139">リストに関する追加の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-139">Provides additional details about the list.</span></span>
| <span data-ttu-id="a5a4a-140">**system**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-140">**system**</span></span>       | <span data-ttu-id="a5a4a-141">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-141">[systemFacet][]</span></span>                  | <span data-ttu-id="a5a4a-142">存在する場合は、これがシステム管理のリストであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-142">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="a5a4a-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-143">Read-only.</span></span>

<span data-ttu-id="a5a4a-144">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="a5a4a-145">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a5a4a-145">Property name</span></span>            | <span data-ttu-id="a5a4a-146">Type</span><span class="sxs-lookup"><span data-stu-id="a5a4a-146">Type</span></span>              | <span data-ttu-id="a5a4a-147">説明</span><span class="sxs-lookup"><span data-stu-id="a5a4a-147">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="a5a4a-148">**id**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-148">**id**</span></span>                   | <span data-ttu-id="a5a4a-149">string</span><span class="sxs-lookup"><span data-stu-id="a5a4a-149">string</span></span>            | <span data-ttu-id="a5a4a-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="a5a4a-152">**name**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-152">**name**</span></span>                 | <span data-ttu-id="a5a4a-153">文字列</span><span class="sxs-lookup"><span data-stu-id="a5a4a-153">string</span></span>            | <span data-ttu-id="a5a4a-154">アイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-154">The name of the item.</span></span>
| <span data-ttu-id="a5a4a-155">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-155">**createdBy**</span></span>            | <span data-ttu-id="a5a4a-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-156">[identitySet][]</span></span>   | <span data-ttu-id="a5a4a-157">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-157">Identity of the creator of this item.</span></span> <span data-ttu-id="a5a4a-158">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-158">Read-only.</span></span>
| <span data-ttu-id="a5a4a-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-159">**createdDateTime**</span></span>      | <span data-ttu-id="a5a4a-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5a4a-160">DateTimeOffset</span></span>    | <span data-ttu-id="a5a4a-p106">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="a5a4a-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-163">**description**</span></span>          | <span data-ttu-id="a5a4a-164">文字列</span><span class="sxs-lookup"><span data-stu-id="a5a4a-164">string</span></span>            | <span data-ttu-id="a5a4a-165">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="a5a4a-166">**eTag**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-166">**eTag**</span></span>                 | <span data-ttu-id="a5a4a-167">文字列</span><span class="sxs-lookup"><span data-stu-id="a5a4a-167">string</span></span>            | <span data-ttu-id="a5a4a-p107">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="a5a4a-170">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-170">**lastModifiedBy**</span></span>       | <span data-ttu-id="a5a4a-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-171">[identitySet][]</span></span>   | <span data-ttu-id="a5a4a-172">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="a5a4a-173">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-173">Read-only.</span></span>
| <span data-ttu-id="a5a4a-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="a5a4a-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5a4a-175">DateTimeOffset</span></span>    | <span data-ttu-id="a5a4a-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="a5a4a-178">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-178">**parentReference**</span></span>      | <span data-ttu-id="a5a4a-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-179">[itemReference][]</span></span> | <span data-ttu-id="a5a4a-p110">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="a5a4a-182">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-182">**sharepointIds**</span></span>        | <span data-ttu-id="a5a4a-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-183">[sharepointIds][]</span></span> | <span data-ttu-id="a5a4a-p111">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="a5a4a-186">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-186">**webUrl**</span></span>               | <span data-ttu-id="a5a4a-187">string (URL)</span><span class="sxs-lookup"><span data-stu-id="a5a4a-187">string (url)</span></span>      | <span data-ttu-id="a5a4a-p112">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="a5a4a-190">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a5a4a-190">Relationships</span></span>

<span data-ttu-id="a5a4a-191">**list** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-191">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="a5a4a-192">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="a5a4a-192">Relationship name</span></span> | <span data-ttu-id="a5a4a-193">種類</span><span class="sxs-lookup"><span data-stu-id="a5a4a-193">Type</span></span>                             | <span data-ttu-id="a5a4a-194">説明</span><span class="sxs-lookup"><span data-stu-id="a5a4a-194">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="a5a4a-195">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-195">**drive**</span></span>         | <span data-ttu-id="a5a4a-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="a5a4a-196">[drive][]</span></span>                        | <span data-ttu-id="a5a4a-197">ドキュメント ライブラリにのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-197">Only present on document libraries.</span></span> <span data-ttu-id="a5a4a-198">[driveItems][driveItem] を含む [drive][] リソースとしてリストにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="a5a4a-199">**items**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-199">**items**</span></span>         | <span data-ttu-id="a5a4a-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="a5a4a-200">Collection([listItem][])</span></span>         | <span data-ttu-id="a5a4a-201">リストに含まれているすべてのアイテム。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-201">All items contained in the list.</span></span>
| <span data-ttu-id="a5a4a-202">**columns**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-202">**columns**</span></span>       | <span data-ttu-id="a5a4a-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="a5a4a-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="a5a4a-204">このリストのフィールド定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-204">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="a5a4a-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="a5a4a-205">**contentTypes**</span></span>  | <span data-ttu-id="a5a4a-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="a5a4a-206">Collection([contentType][])</span></span>      | <span data-ttu-id="a5a4a-207">このリスト内に存在するコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a5a4a-207">The collection of content types present in this list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[sharepointIds]: sharepointids.md
[site]: site.md
[systemFacet]: systemfacet.md

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
