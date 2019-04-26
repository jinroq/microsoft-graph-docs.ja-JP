---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: List
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 7946346c5b872cad80eb3b8dc50109862ac15b8e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570800"
---
# <a name="list-resource"></a><span data-ttu-id="09b7f-102">List リソース</span><span class="sxs-lookup"><span data-stu-id="09b7f-102">List resource</span></span>

<span data-ttu-id="09b7f-103">**list** リソースは [site][] 内のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="09b7f-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="09b7f-104">このリソースには、テンプレートとフィールドの定義を含め、リストの最上位レベルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="09b7f-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="09b7f-105">リスト上のタスク</span><span class="sxs-lookup"><span data-stu-id="09b7f-105">Tasks on a list</span></span>

<span data-ttu-id="09b7f-106">list リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="09b7f-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="09b7f-107">**注:** このベータ版では、リスト上の移動だけが可能であり、リストの作成や更新はできません。</span><span class="sxs-lookup"><span data-stu-id="09b7f-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="09b7f-108">ただし、[リスト アイテム]の [listItem] の作成または更新は可能です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="09b7f-109">以下のすべての例は、`https://graph.microsoft.com/v1.0/sites/{site-id}` などのサイトからの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="09b7f-110">共通タスク</span><span class="sxs-lookup"><span data-stu-id="09b7f-110">Common task</span></span>               | <span data-ttu-id="09b7f-111">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="09b7f-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="09b7f-112">[リストを取得する][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-112">[Get list][]</span></span>              | <span data-ttu-id="09b7f-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="09b7f-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="09b7f-114">[リスト アイテムを列挙する][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="09b7f-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="09b7f-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="09b7f-116">[リスト アイテムを更新する][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-116">[Update list item][]</span></span>      | <span data-ttu-id="09b7f-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="09b7f-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="09b7f-118">[リスト アイテムを削除する][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-118">[Delete list item][]</span></span>      | <span data-ttu-id="09b7f-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="09b7f-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="09b7f-120">[リスト アイテムを作成する][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-120">[Create list item][]</span></span>      | <span data-ttu-id="09b7f-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="09b7f-121">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="09b7f-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09b7f-127">JSON representation</span></span>

<span data-ttu-id="09b7f-128">以下は、**list** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-128">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="09b7f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09b7f-129">Properties</span></span>

<span data-ttu-id="09b7f-130">**list** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="09b7f-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="09b7f-131">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="09b7f-131">Property name</span></span>    | <span data-ttu-id="09b7f-132">種類</span><span class="sxs-lookup"><span data-stu-id="09b7f-132">Type</span></span>                             | <span data-ttu-id="09b7f-133">説明</span><span class="sxs-lookup"><span data-stu-id="09b7f-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="09b7f-134">**displayName**</span><span class="sxs-lookup"><span data-stu-id="09b7f-134">**displayName**</span></span>  | <span data-ttu-id="09b7f-135">string</span><span class="sxs-lookup"><span data-stu-id="09b7f-135">string</span></span>                           | <span data-ttu-id="09b7f-136">リストの表示可能なタイトルです。</span><span class="sxs-lookup"><span data-stu-id="09b7f-136">The displayable title of the list.</span></span>
| <span data-ttu-id="09b7f-137">**list**</span><span class="sxs-lookup"><span data-stu-id="09b7f-137">**list**</span></span>         | <span data-ttu-id="09b7f-138">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-138">[listInfo][]</span></span>                     | <span data-ttu-id="09b7f-139">リストに関する追加の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="09b7f-139">Provides additional details about the list.</span></span>
| <span data-ttu-id="09b7f-140">**system**</span><span class="sxs-lookup"><span data-stu-id="09b7f-140">**system**</span></span>       | <span data-ttu-id="09b7f-141">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-141">[systemFacet][]</span></span>                  | <span data-ttu-id="09b7f-142">存在する場合は、これがシステム管理のリストであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="09b7f-142">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="09b7f-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-143">Read-only.</span></span>

<span data-ttu-id="09b7f-144">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="09b7f-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="09b7f-145">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="09b7f-145">Property name</span></span>            | <span data-ttu-id="09b7f-146">種類</span><span class="sxs-lookup"><span data-stu-id="09b7f-146">Type</span></span>              | <span data-ttu-id="09b7f-147">説明</span><span class="sxs-lookup"><span data-stu-id="09b7f-147">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="09b7f-148">**id**</span><span class="sxs-lookup"><span data-stu-id="09b7f-148">**id**</span></span>                   | <span data-ttu-id="09b7f-149">string</span><span class="sxs-lookup"><span data-stu-id="09b7f-149">string</span></span>            | <span data-ttu-id="09b7f-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="09b7f-152">**name**</span><span class="sxs-lookup"><span data-stu-id="09b7f-152">**name**</span></span>                 | <span data-ttu-id="09b7f-153">string</span><span class="sxs-lookup"><span data-stu-id="09b7f-153">string</span></span>            | <span data-ttu-id="09b7f-154">アイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="09b7f-154">The name of the item.</span></span>
| <span data-ttu-id="09b7f-155">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="09b7f-155">**createdBy**</span></span>            | <span data-ttu-id="09b7f-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-156">[identitySet][]</span></span>   | <span data-ttu-id="09b7f-157">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-157">Identity of the creator of this item.</span></span> <span data-ttu-id="09b7f-158">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-158">Read-only.</span></span>
| <span data-ttu-id="09b7f-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="09b7f-159">**createdDateTime**</span></span>      | <span data-ttu-id="09b7f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09b7f-160">DateTimeOffset</span></span>    | <span data-ttu-id="09b7f-p106">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="09b7f-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="09b7f-163">**description**</span></span>          | <span data-ttu-id="09b7f-164">string</span><span class="sxs-lookup"><span data-stu-id="09b7f-164">string</span></span>            | <span data-ttu-id="09b7f-165">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="09b7f-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="09b7f-166">**eTag**</span><span class="sxs-lookup"><span data-stu-id="09b7f-166">**eTag**</span></span>                 | <span data-ttu-id="09b7f-167">string</span><span class="sxs-lookup"><span data-stu-id="09b7f-167">string</span></span>            | <span data-ttu-id="09b7f-p107">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="09b7f-170">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="09b7f-170">**lastModifiedBy**</span></span>       | <span data-ttu-id="09b7f-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-171">[identitySet][]</span></span>   | <span data-ttu-id="09b7f-172">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="09b7f-173">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-173">Read-only.</span></span>
| <span data-ttu-id="09b7f-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="09b7f-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="09b7f-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09b7f-175">DateTimeOffset</span></span>    | <span data-ttu-id="09b7f-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="09b7f-178">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="09b7f-178">**parentReference**</span></span>      | <span data-ttu-id="09b7f-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-179">[itemReference][]</span></span> | <span data-ttu-id="09b7f-p110">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="09b7f-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="09b7f-182">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="09b7f-182">**sharepointIds**</span></span>        | <span data-ttu-id="09b7f-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-183">[sharepointIds][]</span></span> | <span data-ttu-id="09b7f-p111">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="09b7f-186">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="09b7f-186">**webUrl**</span></span>               | <span data-ttu-id="09b7f-187">string (URL)</span><span class="sxs-lookup"><span data-stu-id="09b7f-187">string (url)</span></span>      | <span data-ttu-id="09b7f-p112">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09b7f-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="09b7f-190">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09b7f-190">Relationships</span></span>

<span data-ttu-id="09b7f-191">**list** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="09b7f-191">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="09b7f-192">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="09b7f-192">Relationship name</span></span> | <span data-ttu-id="09b7f-193">種類</span><span class="sxs-lookup"><span data-stu-id="09b7f-193">Type</span></span>                             | <span data-ttu-id="09b7f-194">説明</span><span class="sxs-lookup"><span data-stu-id="09b7f-194">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="09b7f-195">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="09b7f-195">**drive**</span></span>         | <span data-ttu-id="09b7f-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="09b7f-196">[drive][]</span></span>                        | <span data-ttu-id="09b7f-197">ドキュメント ライブラリにのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="09b7f-197">Only present on document libraries.</span></span> <span data-ttu-id="09b7f-198">[driveItems][driveItem] を含む [drive][] リソースとしてリストにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="09b7f-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="09b7f-199">**items**</span><span class="sxs-lookup"><span data-stu-id="09b7f-199">**items**</span></span>         | <span data-ttu-id="09b7f-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="09b7f-200">Collection([listItem][])</span></span>         | <span data-ttu-id="09b7f-201">リストに含まれているすべてのアイテム。</span><span class="sxs-lookup"><span data-stu-id="09b7f-201">All items contained in the list.</span></span>
| <span data-ttu-id="09b7f-202">**列**</span><span class="sxs-lookup"><span data-stu-id="09b7f-202">**columns**</span></span>       | <span data-ttu-id="09b7f-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="09b7f-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="09b7f-204">このリストのフィールド定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="09b7f-204">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="09b7f-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="09b7f-205">**contentTypes**</span></span>  | <span data-ttu-id="09b7f-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="09b7f-206">Collection([contentType][])</span></span>      | <span data-ttu-id="09b7f-207">このリスト内に存在するコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="09b7f-207">The collection of content types present in this list.</span></span>

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
[サイト]: site.md
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
