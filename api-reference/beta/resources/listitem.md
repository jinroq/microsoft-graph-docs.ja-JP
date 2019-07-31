---
author: JeremyKelley
description: このリソースは、SharePoint の list 内のアイテムを表します。
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3c05125257eeec9d7b21a7d1eb03de79bc189ccd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009980"
---
# <a name="listitem-resource"></a><span data-ttu-id="9f0c3-103">ListItem リソース</span><span class="sxs-lookup"><span data-stu-id="9f0c3-103">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f0c3-104">このリソースは、SharePoint の **[list][]** 内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-104">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="9f0c3-105">リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="9f0c3-106">listItem に関するタスク</span><span class="sxs-lookup"><span data-stu-id="9f0c3-106">Tasks on a listItem</span></span>

<span data-ttu-id="9f0c3-107">**listItem** リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-107">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="9f0c3-108">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}` などの**[list][]** からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-108">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="9f0c3-109">共通タスク</span><span class="sxs-lookup"><span data-stu-id="9f0c3-109">Common task</span></span>                    | <span data-ttu-id="9f0c3-110">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="9f0c3-110">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="9f0c3-111">[取得][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-111">[Get][]</span></span>                        | <span data-ttu-id="9f0c3-112">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="9f0c3-112">GET /items/{item-id}</span></span>
| <span data-ttu-id="9f0c3-113">[列の値の取得][取得]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-113">[Get column values][Get]</span></span>       | <span data-ttu-id="9f0c3-114">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="9f0c3-114">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="9f0c3-115">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-115">[Get analytics][]</span></span>              | <span data-ttu-id="9f0c3-116">アイテムを取得する (英語)</span><span class="sxs-lookup"><span data-stu-id="9f0c3-116">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="9f0c3-117">[間隔によりアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-117">[Get activities by interval][]</span></span> | <span data-ttu-id="9f0c3-118">/Items/{item-id}/getActivitiesByInterval を取得する</span><span class="sxs-lookup"><span data-stu-id="9f0c3-118">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="9f0c3-119">[作成][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-119">[Create][]</span></span>                     | <span data-ttu-id="9f0c3-120">POST /items</span><span class="sxs-lookup"><span data-stu-id="9f0c3-120">POST /items</span></span>
| <span data-ttu-id="9f0c3-121">[削除][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-121">[Delete][]</span></span>                     | <span data-ttu-id="9f0c3-122">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="9f0c3-122">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="9f0c3-123">[更新][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-123">[Update][]</span></span>                     | <span data-ttu-id="9f0c3-124">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="9f0c3-124">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="9f0c3-125">[列の値の更新][更新]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-125">[Update column values][Update]</span></span> | <span data-ttu-id="9f0c3-126">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="9f0c3-126">PATCH /items/{item-id}/fields</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="9f0c3-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f0c3-133">JSON representation</span></span>

<span data-ttu-id="9f0c3-134">以下は、**listItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-134">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9f0c3-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f0c3-135">Properties</span></span>

<span data-ttu-id="9f0c3-136">**listItem** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-136">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="9f0c3-137">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9f0c3-137">Property name</span></span> | <span data-ttu-id="9f0c3-138">種類</span><span class="sxs-lookup"><span data-stu-id="9f0c3-138">Type</span></span>                | <span data-ttu-id="9f0c3-139">説明</span><span class="sxs-lookup"><span data-stu-id="9f0c3-139">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="9f0c3-140">contentType</span><span class="sxs-lookup"><span data-stu-id="9f0c3-140">contentType</span></span>   | <span data-ttu-id="9f0c3-141">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-141">[contentTypeInfo][]</span></span> | <span data-ttu-id="9f0c3-142">このリスト アイテムのコンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="9f0c3-142">The content type of this list item</span></span>

<span data-ttu-id="9f0c3-143">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-143">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="9f0c3-144">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9f0c3-144">Property name</span></span>        | <span data-ttu-id="9f0c3-145">種類</span><span class="sxs-lookup"><span data-stu-id="9f0c3-145">Type</span></span>              | <span data-ttu-id="9f0c3-146">説明</span><span class="sxs-lookup"><span data-stu-id="9f0c3-146">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="9f0c3-147">id</span><span class="sxs-lookup"><span data-stu-id="9f0c3-147">id</span></span>                   | <span data-ttu-id="9f0c3-148">string</span><span class="sxs-lookup"><span data-stu-id="9f0c3-148">string</span></span>            | <span data-ttu-id="9f0c3-p103">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="9f0c3-151">name</span><span class="sxs-lookup"><span data-stu-id="9f0c3-151">name</span></span>                 | <span data-ttu-id="9f0c3-152">string</span><span class="sxs-lookup"><span data-stu-id="9f0c3-152">string</span></span>            | <span data-ttu-id="9f0c3-153">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-153">The name / title of the item.</span></span>
| <span data-ttu-id="9f0c3-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="9f0c3-154">createdBy</span></span>            | <span data-ttu-id="9f0c3-155">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-155">[identitySet][]</span></span>   | <span data-ttu-id="9f0c3-156">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-156">Identity of the creator of this item.</span></span> <span data-ttu-id="9f0c3-157">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-157">Read-only.</span></span>
| <span data-ttu-id="9f0c3-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f0c3-158">createdDateTime</span></span>      | <span data-ttu-id="9f0c3-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f0c3-159">DateTimeOffset</span></span>    | <span data-ttu-id="9f0c3-p105">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="9f0c3-162">description</span><span class="sxs-lookup"><span data-stu-id="9f0c3-162">description</span></span>          | <span data-ttu-id="9f0c3-163">string</span><span class="sxs-lookup"><span data-stu-id="9f0c3-163">string</span></span>            | <span data-ttu-id="9f0c3-164">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-164">The descriptive text for the item.</span></span>
| <span data-ttu-id="9f0c3-165">eTag</span><span class="sxs-lookup"><span data-stu-id="9f0c3-165">eTag</span></span>                 | <span data-ttu-id="9f0c3-166">string</span><span class="sxs-lookup"><span data-stu-id="9f0c3-166">string</span></span>            | <span data-ttu-id="9f0c3-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="9f0c3-169">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9f0c3-169">lastModifiedBy</span></span>       | <span data-ttu-id="9f0c3-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-170">[identitySet][]</span></span>   | <span data-ttu-id="9f0c3-171">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-171">Identity of the last modifier of this item.</span></span> <span data-ttu-id="9f0c3-172">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-172">Read-only.</span></span>
| <span data-ttu-id="9f0c3-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f0c3-173">lastModifiedDateTime</span></span> | <span data-ttu-id="9f0c3-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f0c3-174">DateTimeOffset</span></span>    | <span data-ttu-id="9f0c3-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="9f0c3-177">parentReference</span><span class="sxs-lookup"><span data-stu-id="9f0c3-177">parentReference</span></span>      | <span data-ttu-id="9f0c3-178">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-178">[itemReference][]</span></span> | <span data-ttu-id="9f0c3-p109">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="9f0c3-181">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="9f0c3-181">sharepointIds</span></span>        | <span data-ttu-id="9f0c3-182">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-182">[sharepointIds][]</span></span> | <span data-ttu-id="9f0c3-p110">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="9f0c3-185">webUrl</span><span class="sxs-lookup"><span data-stu-id="9f0c3-185">webUrl</span></span>               | <span data-ttu-id="9f0c3-186">string (URL)</span><span class="sxs-lookup"><span data-stu-id="9f0c3-186">string (url)</span></span>      | <span data-ttu-id="9f0c3-p111">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="9f0c3-189">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f0c3-189">Relationships</span></span>

 <span data-ttu-id="9f0c3-190">**listItem** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-190">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="9f0c3-191">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="9f0c3-191">Relationship name</span></span> | <span data-ttu-id="9f0c3-192">種類</span><span class="sxs-lookup"><span data-stu-id="9f0c3-192">Type</span></span>                           | <span data-ttu-id="9f0c3-193">説明</span><span class="sxs-lookup"><span data-stu-id="9f0c3-193">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="9f0c3-194">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="9f0c3-194">activities</span></span>        | <span data-ttu-id="9f0c3-195">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="9f0c3-195">[itemActivity][] collection</span></span>    | <span data-ttu-id="9f0c3-196">このアイテムに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-196">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="9f0c3-197">分析</span><span class="sxs-lookup"><span data-stu-id="9f0c3-197">analytics</span></span>         | <span data-ttu-id="9f0c3-198">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="9f0c3-198">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="9f0c3-199">このアイテムについて行われたビュー アクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-199">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="9f0c3-200">driveItem</span><span class="sxs-lookup"><span data-stu-id="9f0c3-200">driveItem</span></span>         | <span data-ttu-id="9f0c3-201">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-201">[driveItem][]</span></span>                  | <span data-ttu-id="9f0c3-202">ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-202">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="9f0c3-203">フィールド</span><span class="sxs-lookup"><span data-stu-id="9f0c3-203">fields</span></span>            | <span data-ttu-id="9f0c3-204">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="9f0c3-204">[fieldValueSet][]</span></span>              | <span data-ttu-id="9f0c3-205">このリスト アイテムの列セットの値です。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-205">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="9f0c3-206">versions</span><span class="sxs-lookup"><span data-stu-id="9f0c3-206">versions</span></span>          | <span data-ttu-id="9f0c3-207">[listItemVersion][] コレクション</span><span class="sxs-lookup"><span data-stu-id="9f0c3-207">[listItemVersion][] collection</span></span> | <span data-ttu-id="9f0c3-208">リスト アイテムの以前のバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="9f0c3-208">The list of previous versions of the list item.</span></span>

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
