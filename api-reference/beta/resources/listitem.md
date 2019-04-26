---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9f813511ffa8a033d2ee85f8c7e5d2d5a271dd1e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345247"
---
# <a name="listitem-resource"></a><span data-ttu-id="988ed-102">ListItem リソース</span><span class="sxs-lookup"><span data-stu-id="988ed-102">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="988ed-103">このリソースは、SharePoint の **[list][]** 内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="988ed-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="988ed-104">リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。</span><span class="sxs-lookup"><span data-stu-id="988ed-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="988ed-105">listItem に関するタスク</span><span class="sxs-lookup"><span data-stu-id="988ed-105">Tasks on a listItem</span></span>

<span data-ttu-id="988ed-106">**listItem** リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="988ed-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="988ed-107">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}` などの**[list][]** からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="988ed-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="988ed-108">共通タスク</span><span class="sxs-lookup"><span data-stu-id="988ed-108">Common task</span></span>                    | <span data-ttu-id="988ed-109">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="988ed-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="988ed-110">[取得][]</span><span class="sxs-lookup"><span data-stu-id="988ed-110">[Get][]</span></span>                        | <span data-ttu-id="988ed-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="988ed-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="988ed-112">[列の値の取得][取得]</span><span class="sxs-lookup"><span data-stu-id="988ed-112">[Get column values][Get]</span></span>       | <span data-ttu-id="988ed-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="988ed-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="988ed-114">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="988ed-114">[Get analytics][]</span></span>              | <span data-ttu-id="988ed-115">アイテムを取得する (英語)</span><span class="sxs-lookup"><span data-stu-id="988ed-115">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="988ed-116">[間隔によりアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="988ed-116">[Get activities by interval][]</span></span> | <span data-ttu-id="988ed-117">/items/{item-id}/getActivitiesByInterval を取得する</span><span class="sxs-lookup"><span data-stu-id="988ed-117">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="988ed-118">[作成][]</span><span class="sxs-lookup"><span data-stu-id="988ed-118">[Create][]</span></span>                     | <span data-ttu-id="988ed-119">POST /items</span><span class="sxs-lookup"><span data-stu-id="988ed-119">POST /items</span></span>
| <span data-ttu-id="988ed-120">[削除][]</span><span class="sxs-lookup"><span data-stu-id="988ed-120">[Delete][]</span></span>                     | <span data-ttu-id="988ed-121">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="988ed-121">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="988ed-122">[更新][]</span><span class="sxs-lookup"><span data-stu-id="988ed-122">[Update][]</span></span>                     | <span data-ttu-id="988ed-123">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="988ed-123">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="988ed-124">[列の値の更新][更新]</span><span class="sxs-lookup"><span data-stu-id="988ed-124">[Update column values][Update]</span></span> | <span data-ttu-id="988ed-125">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="988ed-125">PATCH /items/{item-id}/fields</span></span>

[取得]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[分析を取得する]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔によりアクティビティを取得する]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[更新]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="988ed-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="988ed-132">JSON representation</span></span>

<span data-ttu-id="988ed-133">以下は、**listItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="988ed-133">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="988ed-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="988ed-134">Properties</span></span>

<span data-ttu-id="988ed-135">**listItem** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="988ed-135">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="988ed-136">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="988ed-136">Property name</span></span> | <span data-ttu-id="988ed-137">種類</span><span class="sxs-lookup"><span data-stu-id="988ed-137">Type</span></span>                | <span data-ttu-id="988ed-138">説明</span><span class="sxs-lookup"><span data-stu-id="988ed-138">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="988ed-139">contentType</span><span class="sxs-lookup"><span data-stu-id="988ed-139">contentType</span></span>   | <span data-ttu-id="988ed-140">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="988ed-140">[contentTypeInfo][]</span></span> | <span data-ttu-id="988ed-141">このリスト アイテムのコンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="988ed-141">The content type of this list item</span></span>

<span data-ttu-id="988ed-142">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="988ed-142">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="988ed-143">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="988ed-143">Property name</span></span>        | <span data-ttu-id="988ed-144">種類</span><span class="sxs-lookup"><span data-stu-id="988ed-144">Type</span></span>              | <span data-ttu-id="988ed-145">説明</span><span class="sxs-lookup"><span data-stu-id="988ed-145">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="988ed-146">id</span><span class="sxs-lookup"><span data-stu-id="988ed-146">id</span></span>                   | <span data-ttu-id="988ed-147">string</span><span class="sxs-lookup"><span data-stu-id="988ed-147">string</span></span>            | <span data-ttu-id="988ed-p103">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ed-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="988ed-150">name</span><span class="sxs-lookup"><span data-stu-id="988ed-150">name</span></span>                 | <span data-ttu-id="988ed-151">string</span><span class="sxs-lookup"><span data-stu-id="988ed-151">string</span></span>            | <span data-ttu-id="988ed-152">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="988ed-152">The name / title of the item.</span></span>
| <span data-ttu-id="988ed-153">createdBy</span><span class="sxs-lookup"><span data-stu-id="988ed-153">createdBy</span></span>            | <span data-ttu-id="988ed-154">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="988ed-154">[identitySet][]</span></span>   | <span data-ttu-id="988ed-155">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="988ed-155">Identity of the creator of this item.</span></span> <span data-ttu-id="988ed-156">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ed-156">Read-only.</span></span>
| <span data-ttu-id="988ed-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="988ed-157">createdDateTime</span></span>      | <span data-ttu-id="988ed-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="988ed-158">DateTimeOffset</span></span>    | <span data-ttu-id="988ed-p105">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ed-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="988ed-161">description</span><span class="sxs-lookup"><span data-stu-id="988ed-161">description</span></span>          | <span data-ttu-id="988ed-162">string</span><span class="sxs-lookup"><span data-stu-id="988ed-162">string</span></span>            | <span data-ttu-id="988ed-163">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="988ed-163">The descriptive text for the item.</span></span>
| <span data-ttu-id="988ed-164">eTag</span><span class="sxs-lookup"><span data-stu-id="988ed-164">eTag</span></span>                 | <span data-ttu-id="988ed-165">string</span><span class="sxs-lookup"><span data-stu-id="988ed-165">string</span></span>            | <span data-ttu-id="988ed-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ed-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="988ed-168">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="988ed-168">lastModifiedBy</span></span>       | <span data-ttu-id="988ed-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="988ed-169">[identitySet][]</span></span>   | <span data-ttu-id="988ed-170">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="988ed-170">Identity of the last modifier of this item.</span></span> <span data-ttu-id="988ed-171">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ed-171">Read-only.</span></span>
| <span data-ttu-id="988ed-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="988ed-172">lastModifiedDateTime</span></span> | <span data-ttu-id="988ed-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="988ed-173">DateTimeOffset</span></span>    | <span data-ttu-id="988ed-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ed-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="988ed-176">parentReference</span><span class="sxs-lookup"><span data-stu-id="988ed-176">parentReference</span></span>      | <span data-ttu-id="988ed-177">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="988ed-177">[itemReference][]</span></span> | <span data-ttu-id="988ed-p109">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="988ed-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="988ed-180">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="988ed-180">sharepointIds</span></span>        | <span data-ttu-id="988ed-181">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="988ed-181">[sharepointIds][]</span></span> | <span data-ttu-id="988ed-p110">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ed-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="988ed-184">webUrl</span><span class="sxs-lookup"><span data-stu-id="988ed-184">webUrl</span></span>               | <span data-ttu-id="988ed-185">string (URL)</span><span class="sxs-lookup"><span data-stu-id="988ed-185">string (url)</span></span>      | <span data-ttu-id="988ed-p111">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="988ed-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="988ed-188">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="988ed-188">Relationships</span></span>

 <span data-ttu-id="988ed-189">**listItem** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="988ed-189">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="988ed-190">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="988ed-190">Relationship name</span></span> | <span data-ttu-id="988ed-191">種類</span><span class="sxs-lookup"><span data-stu-id="988ed-191">Type</span></span>                           | <span data-ttu-id="988ed-192">説明</span><span class="sxs-lookup"><span data-stu-id="988ed-192">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="988ed-193">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="988ed-193">activities</span></span>        | <span data-ttu-id="988ed-194">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="988ed-194">[itemActivity][] collection</span></span>    | <span data-ttu-id="988ed-195">このアイテムに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="988ed-195">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="988ed-196">analytics</span><span class="sxs-lookup"><span data-stu-id="988ed-196">analytics</span></span>         | <span data-ttu-id="988ed-197">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="988ed-197">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="988ed-198">このアイテムに対して行われたビューアクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="988ed-198">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="988ed-199">driveItem</span><span class="sxs-lookup"><span data-stu-id="988ed-199">driveItem</span></span>         | <span data-ttu-id="988ed-200">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="988ed-200">[driveItem][]</span></span>                  | <span data-ttu-id="988ed-201">ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。</span><span class="sxs-lookup"><span data-stu-id="988ed-201">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="988ed-202">フィールド</span><span class="sxs-lookup"><span data-stu-id="988ed-202">fields</span></span>            | <span data-ttu-id="988ed-203">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="988ed-203">[fieldValueSet][]</span></span>              | <span data-ttu-id="988ed-204">このリスト アイテムの列セットの値です。</span><span class="sxs-lookup"><span data-stu-id="988ed-204">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="988ed-205">versions</span><span class="sxs-lookup"><span data-stu-id="988ed-205">versions</span></span>          | <span data-ttu-id="988ed-206">[listItemVersion][] コレクション</span><span class="sxs-lookup"><span data-stu-id="988ed-206">[listItemVersion][] collection</span></span> | <span data-ttu-id="988ed-207">リスト アイテムの以前のバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="988ed-207">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": []
}
-->
