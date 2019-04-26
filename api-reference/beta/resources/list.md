---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5e078c79603235059cbe326c850e51dfa33d2f8e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345338"
---
# <a name="list-resource"></a><span data-ttu-id="f92e5-102">List リソース</span><span class="sxs-lookup"><span data-stu-id="f92e5-102">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f92e5-103">**list** リソースは [site][] 内のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="f92e5-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="f92e5-104">このリソースには、テンプレートとフィールドの定義を含め、リストの最上位レベルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f92e5-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="f92e5-105">リスト上のタスク</span><span class="sxs-lookup"><span data-stu-id="f92e5-105">Tasks on a list</span></span>

<span data-ttu-id="f92e5-106">list リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="f92e5-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="f92e5-107">**注:** このベータ版では、リスト上の移動だけが可能であり、リストの作成や更新はできません。</span><span class="sxs-lookup"><span data-stu-id="f92e5-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="f92e5-108">ただし、[リスト アイテム]の [listItem] の作成または更新は可能です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="f92e5-109">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}` などのサイトからの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="f92e5-110">共通タスク</span><span class="sxs-lookup"><span data-stu-id="f92e5-110">Common task</span></span>               | <span data-ttu-id="f92e5-111">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="f92e5-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="f92e5-112">[リストを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-112">[Get list][]</span></span>              | <span data-ttu-id="f92e5-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="f92e5-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="f92e5-114">[リスト アイテムを列挙する][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="f92e5-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="f92e5-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="f92e5-116">[リスト アイテムを更新する][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-116">[Update list item][]</span></span>      | <span data-ttu-id="f92e5-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f92e5-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="f92e5-118">[リスト アイテムを削除する][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-118">[Delete list item][]</span></span>      | <span data-ttu-id="f92e5-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f92e5-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="f92e5-120">[リスト アイテムを作成する][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-120">[Create list item][]</span></span>      | <span data-ttu-id="f92e5-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="f92e5-121">POST /lists/{list-id}</span></span>
| <span data-ttu-id="f92e5-122">[最近のアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-122">[Get recent activities][]</span></span> | <span data-ttu-id="f92e5-123">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="f92e5-123">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="f92e5-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f92e5-130">JSON representation</span></span>

<span data-ttu-id="f92e5-131">以下は、**list** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-131">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f92e5-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f92e5-132">Properties</span></span>

<span data-ttu-id="f92e5-133">**list** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="f92e5-133">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="f92e5-134">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f92e5-134">Property name</span></span>    | <span data-ttu-id="f92e5-135">種類</span><span class="sxs-lookup"><span data-stu-id="f92e5-135">Type</span></span>                             | <span data-ttu-id="f92e5-136">説明</span><span class="sxs-lookup"><span data-stu-id="f92e5-136">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="f92e5-137">**columns**</span><span class="sxs-lookup"><span data-stu-id="f92e5-137">**columns**</span></span>      | <span data-ttu-id="f92e5-138">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="f92e5-138">Collection([columnDefinition][])</span></span> | <span data-ttu-id="f92e5-139">このリストのフィールド定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f92e5-139">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="f92e5-140">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="f92e5-140">**contentTypes**</span></span> | <span data-ttu-id="f92e5-141">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="f92e5-141">Collection([contentType][])</span></span>      | <span data-ttu-id="f92e5-142">このリスト内に存在するコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f92e5-142">The collection of content types present in this list.</span></span>
| <span data-ttu-id="f92e5-143">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f92e5-143">**displayName**</span></span>  | <span data-ttu-id="f92e5-144">string</span><span class="sxs-lookup"><span data-stu-id="f92e5-144">string</span></span>                           | <span data-ttu-id="f92e5-145">リストの表示可能なタイトルです。</span><span class="sxs-lookup"><span data-stu-id="f92e5-145">The displayable title of the list.</span></span>
| <span data-ttu-id="f92e5-146">**list**</span><span class="sxs-lookup"><span data-stu-id="f92e5-146">**list**</span></span>         | <span data-ttu-id="f92e5-147">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-147">[listInfo][]</span></span>                     | <span data-ttu-id="f92e5-148">リストに関する追加の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="f92e5-148">Provides additional details about the list.</span></span>
| <span data-ttu-id="f92e5-149">**system**</span><span class="sxs-lookup"><span data-stu-id="f92e5-149">**system**</span></span>       | <span data-ttu-id="f92e5-150">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-150">[systemFacet][]</span></span>                  | <span data-ttu-id="f92e5-151">存在する場合は、これがシステム管理のリストであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="f92e5-151">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="f92e5-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-152">Read-only.</span></span>

<span data-ttu-id="f92e5-153">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="f92e5-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="f92e5-154">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f92e5-154">Property name</span></span>            | <span data-ttu-id="f92e5-155">種類</span><span class="sxs-lookup"><span data-stu-id="f92e5-155">Type</span></span>             | <span data-ttu-id="f92e5-156">説明</span><span class="sxs-lookup"><span data-stu-id="f92e5-156">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="f92e5-157">**id**</span><span class="sxs-lookup"><span data-stu-id="f92e5-157">**id**</span></span>                   | <span data-ttu-id="f92e5-158">string</span><span class="sxs-lookup"><span data-stu-id="f92e5-158">string</span></span>           | <span data-ttu-id="f92e5-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f92e5-161">**name**</span><span class="sxs-lookup"><span data-stu-id="f92e5-161">**name**</span></span>                 | <span data-ttu-id="f92e5-162">string</span><span class="sxs-lookup"><span data-stu-id="f92e5-162">string</span></span>           | <span data-ttu-id="f92e5-163">アイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="f92e5-163">The name of the item.</span></span>
| <span data-ttu-id="f92e5-164">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="f92e5-164">**createdBy**</span></span>            | <span data-ttu-id="f92e5-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-165">[identitySet][]</span></span>  | <span data-ttu-id="f92e5-166">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-166">Identity of the creator of this item.</span></span> <span data-ttu-id="f92e5-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-167">Read-only.</span></span>
| <span data-ttu-id="f92e5-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="f92e5-168">**createdDateTime**</span></span>      | <span data-ttu-id="f92e5-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f92e5-169">DateTimeOffset</span></span>   | <span data-ttu-id="f92e5-p106">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f92e5-172">**説明**</span><span class="sxs-lookup"><span data-stu-id="f92e5-172">**description**</span></span>          | <span data-ttu-id="f92e5-173">string</span><span class="sxs-lookup"><span data-stu-id="f92e5-173">string</span></span>           | <span data-ttu-id="f92e5-174">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="f92e5-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="f92e5-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="f92e5-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="f92e5-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-176">[identitySet][]</span></span>  | <span data-ttu-id="f92e5-177">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="f92e5-178">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-178">Read-only.</span></span>
| <span data-ttu-id="f92e5-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f92e5-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="f92e5-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f92e5-180">DateTimeOffset</span></span>   | <span data-ttu-id="f92e5-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f92e5-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="f92e5-183">**webUrl**</span></span>               | <span data-ttu-id="f92e5-184">string (URL)</span><span class="sxs-lookup"><span data-stu-id="f92e5-184">string (url)</span></span>     | <span data-ttu-id="f92e5-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f92e5-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f92e5-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f92e5-187">Relationships</span></span>

<span data-ttu-id="f92e5-188">**list** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="f92e5-188">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="f92e5-189">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="f92e5-189">Relationship name</span></span> | <span data-ttu-id="f92e5-190">種類</span><span class="sxs-lookup"><span data-stu-id="f92e5-190">Type</span></span>                        | <span data-ttu-id="f92e5-191">説明</span><span class="sxs-lookup"><span data-stu-id="f92e5-191">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="f92e5-192">**activities**</span><span class="sxs-lookup"><span data-stu-id="f92e5-192">**activities**</span></span>    | <span data-ttu-id="f92e5-193">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="f92e5-193">[itemActivity][] collection</span></span> | <span data-ttu-id="f92e5-194">このリスト内で行われた最近のアクティビティです。</span><span class="sxs-lookup"><span data-stu-id="f92e5-194">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="f92e5-195">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="f92e5-195">**drive**</span></span>         | <span data-ttu-id="f92e5-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="f92e5-196">[drive][]</span></span>                   | <span data-ttu-id="f92e5-197">ドキュメント ライブラリにのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="f92e5-197">Only present on document libraries.</span></span> <span data-ttu-id="f92e5-198">[driveItems][driveItem] を含む [drive][] リソースとしてリストにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f92e5-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="f92e5-199">**items**</span><span class="sxs-lookup"><span data-stu-id="f92e5-199">**items**</span></span>         | <span data-ttu-id="f92e5-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="f92e5-200">Collection([listItem][])</span></span>    | <span data-ttu-id="f92e5-201">リストに含まれているすべてのアイテム。</span><span class="sxs-lookup"><span data-stu-id="f92e5-201">All items contained in the list.</span></span>

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
