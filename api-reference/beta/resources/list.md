---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: リスト
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: aafae9e9214f98ade129d46b63f0e7f930ac4a9c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481518"
---
# <a name="list-resource"></a><span data-ttu-id="95dd9-102">list リソース</span><span class="sxs-lookup"><span data-stu-id="95dd9-102">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95dd9-103">**list** リソースは [site][] 内のリストを表します。</span><span class="sxs-lookup"><span data-stu-id="95dd9-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="95dd9-104">このリソースには、テンプレートとフィールドの定義を含め、リストの最上位レベルのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="95dd9-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="95dd9-105">リスト上のタスク</span><span class="sxs-lookup"><span data-stu-id="95dd9-105">Tasks on a list</span></span>

<span data-ttu-id="95dd9-106">list リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="95dd9-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="95dd9-107">**注:** このベータ版では、リスト上の移動だけが可能であり、リストの作成や更新はできません。</span><span class="sxs-lookup"><span data-stu-id="95dd9-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="95dd9-108">ただし、[リスト アイテム]の [listItem] の作成または更新は可能です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="95dd9-109">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}` などのサイトからの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="95dd9-110">共通タスク</span><span class="sxs-lookup"><span data-stu-id="95dd9-110">Common task</span></span>               | <span data-ttu-id="95dd9-111">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="95dd9-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="95dd9-112">[リストを取得する][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-112">[Get list][]</span></span>              | <span data-ttu-id="95dd9-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="95dd9-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="95dd9-114">[リスト アイテムを列挙する][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="95dd9-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="95dd9-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="95dd9-116">[リスト アイテムを更新する][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-116">[Update list item][]</span></span>      | <span data-ttu-id="95dd9-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="95dd9-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="95dd9-118">[リスト アイテムを削除する][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-118">[Delete list item][]</span></span>      | <span data-ttu-id="95dd9-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="95dd9-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="95dd9-120">[リスト アイテムを作成する][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-120">[Create list item][]</span></span>      | <span data-ttu-id="95dd9-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="95dd9-121">POST /lists/{list-id}</span></span>
| <span data-ttu-id="95dd9-122">[最近のアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-122">[Get recent activities][]</span></span> | <span data-ttu-id="95dd9-123">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="95dd9-123">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="95dd9-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95dd9-130">JSON representation</span></span>

<span data-ttu-id="95dd9-131">以下は、**list** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-131">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="95dd9-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95dd9-132">Properties</span></span>

<span data-ttu-id="95dd9-133">**list** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="95dd9-133">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="95dd9-134">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="95dd9-134">Property name</span></span>    | <span data-ttu-id="95dd9-135">種類</span><span class="sxs-lookup"><span data-stu-id="95dd9-135">Type</span></span>                             | <span data-ttu-id="95dd9-136">説明</span><span class="sxs-lookup"><span data-stu-id="95dd9-136">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="95dd9-137">**columns**</span><span class="sxs-lookup"><span data-stu-id="95dd9-137">**columns**</span></span>      | <span data-ttu-id="95dd9-138">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="95dd9-138">Collection([columnDefinition][])</span></span> | <span data-ttu-id="95dd9-139">このリストのフィールド定義のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="95dd9-139">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="95dd9-140">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="95dd9-140">**contentTypes**</span></span> | <span data-ttu-id="95dd9-141">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="95dd9-141">Collection([contentType][])</span></span>      | <span data-ttu-id="95dd9-142">このリスト内に存在するコンテンツ タイプのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="95dd9-142">The collection of content types present in this list.</span></span>
| <span data-ttu-id="95dd9-143">**displayName**</span><span class="sxs-lookup"><span data-stu-id="95dd9-143">**displayName**</span></span>  | <span data-ttu-id="95dd9-144">string</span><span class="sxs-lookup"><span data-stu-id="95dd9-144">string</span></span>                           | <span data-ttu-id="95dd9-145">リストの表示可能なタイトルです。</span><span class="sxs-lookup"><span data-stu-id="95dd9-145">The displayable title of the list.</span></span>
| <span data-ttu-id="95dd9-146">**list**</span><span class="sxs-lookup"><span data-stu-id="95dd9-146">**list**</span></span>         | <span data-ttu-id="95dd9-147">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-147">[listInfo][]</span></span>                     | <span data-ttu-id="95dd9-148">リストに関する追加の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="95dd9-148">Provides additional details about the list.</span></span>
| <span data-ttu-id="95dd9-149">**system**</span><span class="sxs-lookup"><span data-stu-id="95dd9-149">**system**</span></span>       | <span data-ttu-id="95dd9-150">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-150">[systemFacet][]</span></span>                  | <span data-ttu-id="95dd9-151">存在する場合は、これがシステム管理のリストであることを示しています。</span><span class="sxs-lookup"><span data-stu-id="95dd9-151">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="95dd9-152">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-152">Read-only.</span></span>

<span data-ttu-id="95dd9-153">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="95dd9-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="95dd9-154">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="95dd9-154">Property name</span></span>            | <span data-ttu-id="95dd9-155">種類</span><span class="sxs-lookup"><span data-stu-id="95dd9-155">Type</span></span>             | <span data-ttu-id="95dd9-156">説明</span><span class="sxs-lookup"><span data-stu-id="95dd9-156">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="95dd9-157">**id**</span><span class="sxs-lookup"><span data-stu-id="95dd9-157">**id**</span></span>                   | <span data-ttu-id="95dd9-158">string</span><span class="sxs-lookup"><span data-stu-id="95dd9-158">string</span></span>           | <span data-ttu-id="95dd9-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="95dd9-161">**name**</span><span class="sxs-lookup"><span data-stu-id="95dd9-161">**name**</span></span>                 | <span data-ttu-id="95dd9-162">string</span><span class="sxs-lookup"><span data-stu-id="95dd9-162">string</span></span>           | <span data-ttu-id="95dd9-163">アイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="95dd9-163">The name of the item.</span></span>
| <span data-ttu-id="95dd9-164">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="95dd9-164">**createdBy**</span></span>            | <span data-ttu-id="95dd9-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-165">[identitySet][]</span></span>  | <span data-ttu-id="95dd9-166">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-166">Identity of the creator of this item.</span></span> <span data-ttu-id="95dd9-167">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-167">Read-only.</span></span>
| <span data-ttu-id="95dd9-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="95dd9-168">**createdDateTime**</span></span>      | <span data-ttu-id="95dd9-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95dd9-169">DateTimeOffset</span></span>   | <span data-ttu-id="95dd9-p106">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="95dd9-172">**説明**</span><span class="sxs-lookup"><span data-stu-id="95dd9-172">**description**</span></span>          | <span data-ttu-id="95dd9-173">string</span><span class="sxs-lookup"><span data-stu-id="95dd9-173">string</span></span>           | <span data-ttu-id="95dd9-174">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="95dd9-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="95dd9-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="95dd9-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="95dd9-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-176">[identitySet][]</span></span>  | <span data-ttu-id="95dd9-177">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="95dd9-178">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-178">Read-only.</span></span>
| <span data-ttu-id="95dd9-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="95dd9-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="95dd9-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95dd9-180">DateTimeOffset</span></span>   | <span data-ttu-id="95dd9-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="95dd9-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="95dd9-183">**webUrl**</span></span>               | <span data-ttu-id="95dd9-184">string (URL)</span><span class="sxs-lookup"><span data-stu-id="95dd9-184">string (url)</span></span>     | <span data-ttu-id="95dd9-p109">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95dd9-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="95dd9-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95dd9-187">Relationships</span></span>

<span data-ttu-id="95dd9-188">**list** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="95dd9-188">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="95dd9-189">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="95dd9-189">Relationship name</span></span> | <span data-ttu-id="95dd9-190">種類</span><span class="sxs-lookup"><span data-stu-id="95dd9-190">Type</span></span>                        | <span data-ttu-id="95dd9-191">説明</span><span class="sxs-lookup"><span data-stu-id="95dd9-191">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="95dd9-192">**activities**</span><span class="sxs-lookup"><span data-stu-id="95dd9-192">**activities**</span></span>    | <span data-ttu-id="95dd9-193">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="95dd9-193">[itemActivity][] collection</span></span> | <span data-ttu-id="95dd9-194">このリスト内で行われた最近のアクティビティです。</span><span class="sxs-lookup"><span data-stu-id="95dd9-194">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="95dd9-195">**ドライブ**</span><span class="sxs-lookup"><span data-stu-id="95dd9-195">**drive**</span></span>         | <span data-ttu-id="95dd9-196">[ドライブ][]</span><span class="sxs-lookup"><span data-stu-id="95dd9-196">[drive][]</span></span>                   | <span data-ttu-id="95dd9-197">ドキュメント ライブラリにのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="95dd9-197">Only present on document libraries.</span></span> <span data-ttu-id="95dd9-198">[driveItems][driveItem] を含む [drive][] リソースとしてリストにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="95dd9-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="95dd9-199">**items**</span><span class="sxs-lookup"><span data-stu-id="95dd9-199">**items**</span></span>         | <span data-ttu-id="95dd9-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="95dd9-200">Collection([listItem][])</span></span>    | <span data-ttu-id="95dd9-201">リストに含まれているすべてのアイテム。</span><span class="sxs-lookup"><span data-stu-id="95dd9-201">All items contained in the list.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
