---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.openlocfilehash: 03121447e0b9d7d091005283ed12ef7d93e68108
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870463"
---
# <a name="list-resource"></a><span data-ttu-id="41c7c-102">list リソース</span><span class="sxs-lookup"><span data-stu-id="41c7c-102">List resource</span></span>

> <span data-ttu-id="41c7c-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="41c7c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41c7c-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41c7c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41c7c-105">**list** リソースは [site][] 内のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="41c7c-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="41c7c-106">このリソースには、テンプレートとフィールドの定義を含め、リストの最上位レベルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="41c7c-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="41c7c-107">リスト上のタスク</span><span class="sxs-lookup"><span data-stu-id="41c7c-107">Tasks on a list</span></span>

<span data-ttu-id="41c7c-108">list リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="41c7c-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="41c7c-109">**注:** このベータ版では、リスト上の移動だけが可能であり、リストの作成や更新はできません。</span><span class="sxs-lookup"><span data-stu-id="41c7c-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="41c7c-110">ただし、[リスト アイテム]の [listItem] の作成または更新は可能です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="41c7c-111">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}` などのサイトからの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="41c7c-112">共通タスク</span><span class="sxs-lookup"><span data-stu-id="41c7c-112">Common task</span></span>               | <span data-ttu-id="41c7c-113">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="41c7c-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="41c7c-114">[リストを取得する][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-114">[Get list][]</span></span>              | <span data-ttu-id="41c7c-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="41c7c-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="41c7c-116">[リスト アイテムを列挙する][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-116">[Enumerate list items][]</span></span>  | <span data-ttu-id="41c7c-117">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="41c7c-117">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="41c7c-118">[リスト アイテムを更新する][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-118">[Update list item][]</span></span>      | <span data-ttu-id="41c7c-119">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="41c7c-119">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="41c7c-120">[リスト アイテムを削除する][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-120">[Delete list item][]</span></span>      | <span data-ttu-id="41c7c-121">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="41c7c-121">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="41c7c-122">[リスト アイテムを作成する][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-122">[Create list item][]</span></span>      | <span data-ttu-id="41c7c-123">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="41c7c-123">POST /lists/{list-id}</span></span>
| <span data-ttu-id="41c7c-124">[最近のアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-124">[Get recent activities][]</span></span> | <span data-ttu-id="41c7c-125">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="41c7c-125">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="41c7c-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41c7c-132">JSON representation</span></span>

<span data-ttu-id="41c7c-133">以下は、**list** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-133">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="41c7c-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41c7c-134">Properties</span></span>

<span data-ttu-id="41c7c-135">**list** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="41c7c-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="41c7c-136">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="41c7c-136">Property name</span></span>    | <span data-ttu-id="41c7c-137">Type</span><span class="sxs-lookup"><span data-stu-id="41c7c-137">Type</span></span>                             | <span data-ttu-id="41c7c-138">説明</span><span class="sxs-lookup"><span data-stu-id="41c7c-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="41c7c-139">**columns**</span><span class="sxs-lookup"><span data-stu-id="41c7c-139">**columns**</span></span>      | <span data-ttu-id="41c7c-140">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="41c7c-140">Collection([columnDefinition][])</span></span> | <span data-ttu-id="41c7c-141">このリストのフィールド定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="41c7c-141">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="41c7c-142">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="41c7c-142">**contentTypes**</span></span> | <span data-ttu-id="41c7c-143">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="41c7c-143">Collection([contentType][])</span></span>      | <span data-ttu-id="41c7c-144">このリスト内に存在するコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="41c7c-144">The collection of content types present in this list.</span></span>
| <span data-ttu-id="41c7c-145">**displayName**</span><span class="sxs-lookup"><span data-stu-id="41c7c-145">**displayName**</span></span>  | <span data-ttu-id="41c7c-146">文字列</span><span class="sxs-lookup"><span data-stu-id="41c7c-146">string</span></span>                           | <span data-ttu-id="41c7c-147">リストの表示可能なタイトルです。</span><span class="sxs-lookup"><span data-stu-id="41c7c-147">The displayable title of the list.</span></span>
| <span data-ttu-id="41c7c-148">**list**</span><span class="sxs-lookup"><span data-stu-id="41c7c-148">**list**</span></span>         | <span data-ttu-id="41c7c-149">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-149">[listInfo][]</span></span>                     | <span data-ttu-id="41c7c-150">リストに関する追加の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="41c7c-150">Provides additional details about the list.</span></span>
| <span data-ttu-id="41c7c-151">**system**</span><span class="sxs-lookup"><span data-stu-id="41c7c-151">**system**</span></span>       | <span data-ttu-id="41c7c-152">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-152">[systemFacet][]</span></span>                  | <span data-ttu-id="41c7c-153">存在する場合は、これがシステム管理のリストであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="41c7c-153">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="41c7c-154">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-154">Read-only.</span></span>

<span data-ttu-id="41c7c-155">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="41c7c-155">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="41c7c-156">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="41c7c-156">Property name</span></span>            | <span data-ttu-id="41c7c-157">Type</span><span class="sxs-lookup"><span data-stu-id="41c7c-157">Type</span></span>             | <span data-ttu-id="41c7c-158">説明</span><span class="sxs-lookup"><span data-stu-id="41c7c-158">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="41c7c-159">**id**</span><span class="sxs-lookup"><span data-stu-id="41c7c-159">**id**</span></span>                   | <span data-ttu-id="41c7c-160">string</span><span class="sxs-lookup"><span data-stu-id="41c7c-160">string</span></span>           | <span data-ttu-id="41c7c-p105">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="41c7c-163">**name**</span><span class="sxs-lookup"><span data-stu-id="41c7c-163">**name**</span></span>                 | <span data-ttu-id="41c7c-164">文字列</span><span class="sxs-lookup"><span data-stu-id="41c7c-164">string</span></span>           | <span data-ttu-id="41c7c-165">アイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="41c7c-165">The name of the item.</span></span>
| <span data-ttu-id="41c7c-166">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="41c7c-166">**createdBy**</span></span>            | <span data-ttu-id="41c7c-167">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-167">[identitySet][]</span></span>  | <span data-ttu-id="41c7c-168">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-168">Identity of the creator of this item.</span></span> <span data-ttu-id="41c7c-169">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-169">Read-only.</span></span>
| <span data-ttu-id="41c7c-170">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="41c7c-170">**createdDateTime**</span></span>      | <span data-ttu-id="41c7c-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41c7c-171">DateTimeOffset</span></span>   | <span data-ttu-id="41c7c-p107">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-p107">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="41c7c-174">**説明**</span><span class="sxs-lookup"><span data-stu-id="41c7c-174">**description**</span></span>          | <span data-ttu-id="41c7c-175">文字列</span><span class="sxs-lookup"><span data-stu-id="41c7c-175">string</span></span>           | <span data-ttu-id="41c7c-176">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="41c7c-176">The descriptive text for the item.</span></span>
| <span data-ttu-id="41c7c-177">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="41c7c-177">**lastModifiedBy**</span></span>       | <span data-ttu-id="41c7c-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-178">[identitySet][]</span></span>  | <span data-ttu-id="41c7c-179">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="41c7c-180">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-180">Read-only.</span></span>
| <span data-ttu-id="41c7c-181">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="41c7c-181">**lastModifiedDateTime**</span></span> | <span data-ttu-id="41c7c-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41c7c-182">DateTimeOffset</span></span>   | <span data-ttu-id="41c7c-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="41c7c-185">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="41c7c-185">**webUrl**</span></span>               | <span data-ttu-id="41c7c-186">string (URL)</span><span class="sxs-lookup"><span data-stu-id="41c7c-186">string (url)</span></span>     | <span data-ttu-id="41c7c-p110">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="41c7c-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="41c7c-189">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41c7c-189">Relationships</span></span>

<span data-ttu-id="41c7c-190">**list** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="41c7c-190">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="41c7c-191">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="41c7c-191">Relationship name</span></span> | <span data-ttu-id="41c7c-192">種類</span><span class="sxs-lookup"><span data-stu-id="41c7c-192">Type</span></span>                        | <span data-ttu-id="41c7c-193">説明</span><span class="sxs-lookup"><span data-stu-id="41c7c-193">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="41c7c-194">**activities**</span><span class="sxs-lookup"><span data-stu-id="41c7c-194">**activities**</span></span>    | <span data-ttu-id="41c7c-195">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="41c7c-195">[itemActivity][] collection</span></span> | <span data-ttu-id="41c7c-196">このリスト内で行われた最近のアクティビティです。</span><span class="sxs-lookup"><span data-stu-id="41c7c-196">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="41c7c-197">**drive**</span><span class="sxs-lookup"><span data-stu-id="41c7c-197">**drive**</span></span>         | <span data-ttu-id="41c7c-198">[drive][]</span><span class="sxs-lookup"><span data-stu-id="41c7c-198">[drive][]</span></span>                   | <span data-ttu-id="41c7c-199">ドキュメント ライブラリにのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="41c7c-199">Only present on document libraries.</span></span> <span data-ttu-id="41c7c-200">[driveItems][driveItem] を含む [drive][] リソースとしてリストにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="41c7c-200">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="41c7c-201">**items**</span><span class="sxs-lookup"><span data-stu-id="41c7c-201">**items**</span></span>         | <span data-ttu-id="41c7c-202">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="41c7c-202">Collection([listItem][])</span></span>    | <span data-ttu-id="41c7c-203">リストに含まれているすべてのアイテム。</span><span class="sxs-lookup"><span data-stu-id="41c7c-203">All items contained in the list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[listInfo]: listinfo.md
[listItem]: listitem.md
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
