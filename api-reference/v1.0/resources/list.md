---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: リスト
localization_priority: Priority
ms.prod: sharepoint
description: list リソースでは、サイト内のリストを表します。
doc_type: resourcePageType
ms.openlocfilehash: 51821bb20188c004af3f2aca868c3cfd953ce19c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036408"
---
# <a name="list-resource"></a><span data-ttu-id="51798-103">List リソース</span><span class="sxs-lookup"><span data-stu-id="51798-103">List resource</span></span>

<span data-ttu-id="51798-104">**list** リソースは [site][] 内のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="51798-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="51798-105">このリソースには、テンプレートとフィールドの定義を含め、リストの最上位レベルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="51798-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="51798-106">リスト上のタスク</span><span class="sxs-lookup"><span data-stu-id="51798-106">Tasks on a list</span></span>

<span data-ttu-id="51798-107">list リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="51798-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="51798-108">**注:** このベータ版では、リスト上の移動だけが可能であり、リストの作成や更新はできません。</span><span class="sxs-lookup"><span data-stu-id="51798-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="51798-109">ただし、[リスト アイテム]の [listItem] の作成または更新は可能です。</span><span class="sxs-lookup"><span data-stu-id="51798-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="51798-110">以下のすべての例は、`https://graph.microsoft.com/v1.0/sites/{site-id}` などのサイトからの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="51798-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="51798-111">共通タスク</span><span class="sxs-lookup"><span data-stu-id="51798-111">Common task</span></span>               | <span data-ttu-id="51798-112">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="51798-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="51798-113">[リストを取得する][]</span><span class="sxs-lookup"><span data-stu-id="51798-113">[Get list][]</span></span>              | <span data-ttu-id="51798-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="51798-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="51798-115">[リスト アイテムを列挙する][]</span><span class="sxs-lookup"><span data-stu-id="51798-115">[Enumerate list items][]</span></span>  | <span data-ttu-id="51798-116">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="51798-116">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="51798-117">[リスト アイテムを更新する][]</span><span class="sxs-lookup"><span data-stu-id="51798-117">[Update list item][]</span></span>      | <span data-ttu-id="51798-118">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="51798-118">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="51798-119">[リスト アイテムを削除する][]</span><span class="sxs-lookup"><span data-stu-id="51798-119">[Delete list item][]</span></span>      | <span data-ttu-id="51798-120">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="51798-120">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="51798-121">[リスト アイテムを作成する][]</span><span class="sxs-lookup"><span data-stu-id="51798-121">[Create list item][]</span></span>      | <span data-ttu-id="51798-122">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="51798-122">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="51798-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51798-128">JSON representation</span></span>

<span data-ttu-id="51798-129">以下は、**list** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51798-129">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="51798-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51798-130">Properties</span></span>

<span data-ttu-id="51798-131">**list** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="51798-131">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="51798-132">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="51798-132">Property name</span></span>    | <span data-ttu-id="51798-133">種類</span><span class="sxs-lookup"><span data-stu-id="51798-133">Type</span></span>                             | <span data-ttu-id="51798-134">説明</span><span class="sxs-lookup"><span data-stu-id="51798-134">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="51798-135">**displayName**</span><span class="sxs-lookup"><span data-stu-id="51798-135">**displayName**</span></span>  | <span data-ttu-id="51798-136">string</span><span class="sxs-lookup"><span data-stu-id="51798-136">string</span></span>                           | <span data-ttu-id="51798-137">リストの表示可能なタイトルです。</span><span class="sxs-lookup"><span data-stu-id="51798-137">The displayable title of the list.</span></span>
| <span data-ttu-id="51798-138">**list**</span><span class="sxs-lookup"><span data-stu-id="51798-138">**list**</span></span>         | <span data-ttu-id="51798-139">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="51798-139">[listInfo][]</span></span>                     | <span data-ttu-id="51798-140">リストに関する追加の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="51798-140">Provides additional details about the list.</span></span>
| <span data-ttu-id="51798-141">**system**</span><span class="sxs-lookup"><span data-stu-id="51798-141">**system**</span></span>       | <span data-ttu-id="51798-142">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="51798-142">[systemFacet][]</span></span>                  | <span data-ttu-id="51798-143">存在する場合は、これがシステム管理のリストであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="51798-143">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="51798-144">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-144">Read-only.</span></span>

<span data-ttu-id="51798-145">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="51798-145">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="51798-146">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="51798-146">Property name</span></span>            | <span data-ttu-id="51798-147">種類</span><span class="sxs-lookup"><span data-stu-id="51798-147">Type</span></span>              | <span data-ttu-id="51798-148">説明</span><span class="sxs-lookup"><span data-stu-id="51798-148">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="51798-149">**id**</span><span class="sxs-lookup"><span data-stu-id="51798-149">**id**</span></span>                   | <span data-ttu-id="51798-150">string</span><span class="sxs-lookup"><span data-stu-id="51798-150">string</span></span>            | <span data-ttu-id="51798-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="51798-153">**name**</span><span class="sxs-lookup"><span data-stu-id="51798-153">**name**</span></span>                 | <span data-ttu-id="51798-154">string</span><span class="sxs-lookup"><span data-stu-id="51798-154">string</span></span>            | <span data-ttu-id="51798-155">アイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="51798-155">The name of the item.</span></span>
| <span data-ttu-id="51798-156">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="51798-156">**createdBy**</span></span>            | <span data-ttu-id="51798-157">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="51798-157">[identitySet][]</span></span>   | <span data-ttu-id="51798-158">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="51798-158">Identity of the creator of this item.</span></span> <span data-ttu-id="51798-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-159">Read-only.</span></span>
| <span data-ttu-id="51798-160">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="51798-160">**createdDateTime**</span></span>      | <span data-ttu-id="51798-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51798-161">DateTimeOffset</span></span>    | <span data-ttu-id="51798-p106">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="51798-164">**説明**</span><span class="sxs-lookup"><span data-stu-id="51798-164">**description**</span></span>          | <span data-ttu-id="51798-165">string</span><span class="sxs-lookup"><span data-stu-id="51798-165">string</span></span>            | <span data-ttu-id="51798-166">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="51798-166">The descriptive text for the item.</span></span>
| <span data-ttu-id="51798-167">**eTag**</span><span class="sxs-lookup"><span data-stu-id="51798-167">**eTag**</span></span>                 | <span data-ttu-id="51798-168">string</span><span class="sxs-lookup"><span data-stu-id="51798-168">string</span></span>            | <span data-ttu-id="51798-p107">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="51798-171">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="51798-171">**lastModifiedBy**</span></span>       | <span data-ttu-id="51798-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="51798-172">[identitySet][]</span></span>   | <span data-ttu-id="51798-173">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="51798-173">Identity of the last modifier of this item.</span></span> <span data-ttu-id="51798-174">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-174">Read-only.</span></span>
| <span data-ttu-id="51798-175">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="51798-175">**lastModifiedDateTime**</span></span> | <span data-ttu-id="51798-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51798-176">DateTimeOffset</span></span>    | <span data-ttu-id="51798-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="51798-179">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="51798-179">**parentReference**</span></span>      | <span data-ttu-id="51798-180">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="51798-180">[itemReference][]</span></span> | <span data-ttu-id="51798-p110">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="51798-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="51798-183">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="51798-183">**sharepointIds**</span></span>        | <span data-ttu-id="51798-184">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="51798-184">[sharepointIds][]</span></span> | <span data-ttu-id="51798-p111">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="51798-187">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="51798-187">**webUrl**</span></span>               | <span data-ttu-id="51798-188">string (URL)</span><span class="sxs-lookup"><span data-stu-id="51798-188">string (url)</span></span>      | <span data-ttu-id="51798-p112">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="51798-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="51798-191">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51798-191">Relationships</span></span>

<span data-ttu-id="51798-192">**list** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="51798-192">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="51798-193">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="51798-193">Relationship name</span></span> | <span data-ttu-id="51798-194">種類</span><span class="sxs-lookup"><span data-stu-id="51798-194">Type</span></span>                             | <span data-ttu-id="51798-195">説明</span><span class="sxs-lookup"><span data-stu-id="51798-195">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="51798-196">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="51798-196">**drive**</span></span>         | <span data-ttu-id="51798-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="51798-197">[drive][]</span></span>                        | <span data-ttu-id="51798-198">ドキュメント ライブラリにのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="51798-198">Only present on document libraries.</span></span> <span data-ttu-id="51798-199">[driveItems][driveItem] で [drive][] リソースとしてリストへのアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="51798-199">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="51798-200">**items**</span><span class="sxs-lookup"><span data-stu-id="51798-200">**items**</span></span>         | <span data-ttu-id="51798-201">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="51798-201">Collection([listItem][])</span></span>         | <span data-ttu-id="51798-202">リストに含まれているすべてのアイテム。</span><span class="sxs-lookup"><span data-stu-id="51798-202">All items contained in the list.</span></span>
| <span data-ttu-id="51798-203">**列**</span><span class="sxs-lookup"><span data-stu-id="51798-203">**columns**</span></span>       | <span data-ttu-id="51798-204">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="51798-204">Collection([columnDefinition][])</span></span> | <span data-ttu-id="51798-205">このリストのフィールド定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="51798-205">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="51798-206">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="51798-206">**contentTypes**</span></span>  | <span data-ttu-id="51798-207">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="51798-207">Collection([contentType][])</span></span>      | <span data-ttu-id="51798-208">このリスト内に存在するコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="51798-208">The collection of content types present in this list.</span></span>

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
