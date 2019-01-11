---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.openlocfilehash: b2e151937d5e8db633edeb5d521d6e0c875b6d78
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866088"
---
# <a name="listitem-resource"></a><span data-ttu-id="db9d6-102">ListItem リソース</span><span class="sxs-lookup"><span data-stu-id="db9d6-102">ListItem resource</span></span>

> <span data-ttu-id="db9d6-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="db9d6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db9d6-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db9d6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db9d6-105">このリソースは、SharePoint の **[list][]** 内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="db9d6-105">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="db9d6-106">リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。</span><span class="sxs-lookup"><span data-stu-id="db9d6-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="db9d6-107">listItem に関するタスク</span><span class="sxs-lookup"><span data-stu-id="db9d6-107">Tasks on a listItem</span></span>

<span data-ttu-id="db9d6-108">**listItem** リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="db9d6-108">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="db9d6-109">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}` などの**[list][]** からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-109">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="db9d6-110">共通タスク</span><span class="sxs-lookup"><span data-stu-id="db9d6-110">Common task</span></span>                    | <span data-ttu-id="db9d6-111">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="db9d6-111">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="db9d6-112">[取得][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-112">[Get][]</span></span>                        | <span data-ttu-id="db9d6-113">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="db9d6-113">GET /items/{item-id}</span></span>
| <span data-ttu-id="db9d6-114">[列の値の取得][取得]</span><span class="sxs-lookup"><span data-stu-id="db9d6-114">[Get column values][Get]</span></span>       | <span data-ttu-id="db9d6-115">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="db9d6-115">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="db9d6-116">[分析を取得します。][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-116">[Get analytics][]</span></span>              | <span data-ttu-id="db9d6-117">GET/items/{アイテム id}/分析</span><span class="sxs-lookup"><span data-stu-id="db9d6-117">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="db9d6-118">[間隔によってアクティビティを取得します。][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-118">[Get activities by interval][]</span></span> | <span data-ttu-id="db9d6-119">GET/items/{アイテム id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="db9d6-119">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="db9d6-120">[作成][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-120">[Create][]</span></span>                     | <span data-ttu-id="db9d6-121">POST /items</span><span class="sxs-lookup"><span data-stu-id="db9d6-121">POST /items</span></span>
| <span data-ttu-id="db9d6-122">[削除][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-122">[Delete][]</span></span>                     | <span data-ttu-id="db9d6-123">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="db9d6-123">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="db9d6-124">[更新][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-124">[Update][]</span></span>                     | <span data-ttu-id="db9d6-125">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="db9d6-125">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="db9d6-126">[列の値の更新][更新]</span><span class="sxs-lookup"><span data-stu-id="db9d6-126">[Update column values][Update]</span></span> | <span data-ttu-id="db9d6-127">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="db9d6-127">PATCH /items/{item-id}/fields</span></span>

[取得]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[分析を取得します。]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔によってアクティビティを取得します。]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[更新]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="db9d6-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db9d6-134">JSON representation</span></span>

<span data-ttu-id="db9d6-135">以下は、**listItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-135">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="db9d6-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db9d6-136">Properties</span></span>

<span data-ttu-id="db9d6-137">**listItem** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="db9d6-137">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="db9d6-138">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="db9d6-138">Property name</span></span> | <span data-ttu-id="db9d6-139">Type</span><span class="sxs-lookup"><span data-stu-id="db9d6-139">Type</span></span>                | <span data-ttu-id="db9d6-140">説明</span><span class="sxs-lookup"><span data-stu-id="db9d6-140">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="db9d6-141">contentType</span><span class="sxs-lookup"><span data-stu-id="db9d6-141">contentType</span></span>   | <span data-ttu-id="db9d6-142">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-142">[contentTypeInfo][]</span></span> | <span data-ttu-id="db9d6-143">このリスト アイテムのコンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="db9d6-143">The content type of this list item</span></span>

<span data-ttu-id="db9d6-144">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="db9d6-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="db9d6-145">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="db9d6-145">Property name</span></span>        | <span data-ttu-id="db9d6-146">Type</span><span class="sxs-lookup"><span data-stu-id="db9d6-146">Type</span></span>              | <span data-ttu-id="db9d6-147">説明</span><span class="sxs-lookup"><span data-stu-id="db9d6-147">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="db9d6-148">ID</span><span class="sxs-lookup"><span data-stu-id="db9d6-148">id</span></span>                   | <span data-ttu-id="db9d6-149">文字列</span><span class="sxs-lookup"><span data-stu-id="db9d6-149">string</span></span>            | <span data-ttu-id="db9d6-p104">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="db9d6-152">name</span><span class="sxs-lookup"><span data-stu-id="db9d6-152">name</span></span>                 | <span data-ttu-id="db9d6-153">文字列</span><span class="sxs-lookup"><span data-stu-id="db9d6-153">string</span></span>            | <span data-ttu-id="db9d6-154">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="db9d6-154">The name / title of the item.</span></span>
| <span data-ttu-id="db9d6-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="db9d6-155">createdBy</span></span>            | <span data-ttu-id="db9d6-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-156">[identitySet][]</span></span>   | <span data-ttu-id="db9d6-157">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-157">Identity of the creator of this item.</span></span> <span data-ttu-id="db9d6-158">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-158">Read-only.</span></span>
| <span data-ttu-id="db9d6-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db9d6-159">createdDateTime</span></span>      | <span data-ttu-id="db9d6-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db9d6-160">DateTimeOffset</span></span>    | <span data-ttu-id="db9d6-p106">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="db9d6-163">description</span><span class="sxs-lookup"><span data-stu-id="db9d6-163">description</span></span>          | <span data-ttu-id="db9d6-164">文字列</span><span class="sxs-lookup"><span data-stu-id="db9d6-164">string</span></span>            | <span data-ttu-id="db9d6-165">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="db9d6-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="db9d6-166">eTag</span><span class="sxs-lookup"><span data-stu-id="db9d6-166">eTag</span></span>                 | <span data-ttu-id="db9d6-167">文字列</span><span class="sxs-lookup"><span data-stu-id="db9d6-167">string</span></span>            | <span data-ttu-id="db9d6-p107">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="db9d6-170">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="db9d6-170">lastModifiedBy</span></span>       | <span data-ttu-id="db9d6-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-171">[identitySet][]</span></span>   | <span data-ttu-id="db9d6-172">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="db9d6-173">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-173">Read-only.</span></span>
| <span data-ttu-id="db9d6-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db9d6-174">lastModifiedDateTime</span></span> | <span data-ttu-id="db9d6-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db9d6-175">DateTimeOffset</span></span>    | <span data-ttu-id="db9d6-p109">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="db9d6-178">parentReference</span><span class="sxs-lookup"><span data-stu-id="db9d6-178">parentReference</span></span>      | <span data-ttu-id="db9d6-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-179">[itemReference][]</span></span> | <span data-ttu-id="db9d6-p110">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="db9d6-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="db9d6-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="db9d6-182">sharepointIds</span></span>        | <span data-ttu-id="db9d6-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-183">[sharepointIds][]</span></span> | <span data-ttu-id="db9d6-p111">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="db9d6-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="db9d6-186">webUrl</span></span>               | <span data-ttu-id="db9d6-187">string (URL)</span><span class="sxs-lookup"><span data-stu-id="db9d6-187">string (url)</span></span>      | <span data-ttu-id="db9d6-p112">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="db9d6-190">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="db9d6-190">Relationships</span></span>

 <span data-ttu-id="db9d6-191">**listItem** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="db9d6-191">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="db9d6-192">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="db9d6-192">Relationship name</span></span> | <span data-ttu-id="db9d6-193">種類</span><span class="sxs-lookup"><span data-stu-id="db9d6-193">Type</span></span>                           | <span data-ttu-id="db9d6-194">説明</span><span class="sxs-lookup"><span data-stu-id="db9d6-194">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="db9d6-195">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="db9d6-195">activities</span></span>        | <span data-ttu-id="db9d6-196">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="db9d6-196">[itemActivity][] collection</span></span>    | <span data-ttu-id="db9d6-197">このアイテムに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="db9d6-197">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="db9d6-198">分析</span><span class="sxs-lookup"><span data-stu-id="db9d6-198">analytics</span></span>         | <span data-ttu-id="db9d6-199">[itemAnalytics][]リソース</span><span class="sxs-lookup"><span data-stu-id="db9d6-199">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="db9d6-200">この項目に対して行われた活動の表示について分析します。</span><span class="sxs-lookup"><span data-stu-id="db9d6-200">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="db9d6-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="db9d6-201">driveItem</span></span>         | <span data-ttu-id="db9d6-202">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-202">[driveItem][]</span></span>                  | <span data-ttu-id="db9d6-203">ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。</span><span class="sxs-lookup"><span data-stu-id="db9d6-203">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="db9d6-204">fields</span><span class="sxs-lookup"><span data-stu-id="db9d6-204">fields</span></span>            | <span data-ttu-id="db9d6-205">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="db9d6-205">[fieldValueSet][]</span></span>              | <span data-ttu-id="db9d6-206">このリスト アイテムの列セットの値です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-206">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="db9d6-207">versions</span><span class="sxs-lookup"><span data-stu-id="db9d6-207">versions</span></span>          | <span data-ttu-id="db9d6-208">[listItemVersion][]コレクション</span><span class="sxs-lookup"><span data-stu-id="db9d6-208">[listItemVersion][] collection</span></span> | <span data-ttu-id="db9d6-209">リスト項目の以前のバージョンの一覧です。</span><span class="sxs-lookup"><span data-stu-id="db9d6-209">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[リスト]: list.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
