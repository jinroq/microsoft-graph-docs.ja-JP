---
author: JeremyKelley
ms.author: JeremyKelley
title: ListItem リソース
description: このリソースは、SharePoint のリスト内のアイテムを表します。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 873ad5961c9cadb444c6fe9f2afec69853cc5d85
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968801"
---
# <a name="listitem-resource"></a><span data-ttu-id="93dd0-103">ListItem リソース</span><span class="sxs-lookup"><span data-stu-id="93dd0-103">ListItem resource</span></span>

<span data-ttu-id="93dd0-104">このリソースは、SharePoint の **[list][]** 内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-104">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="93dd0-105">リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。</span><span class="sxs-lookup"><span data-stu-id="93dd0-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="93dd0-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="93dd0-106">Methods</span></span>

<span data-ttu-id="93dd0-107">**listItem** リソースで使用可能なメソッドを次に示します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-107">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="93dd0-108">すべての例は、`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}` の**[リスト][]** からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-108">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="93dd0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="93dd0-109">Method</span></span>                    | <span data-ttu-id="93dd0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93dd0-110">Return Type</span></span> | <span data-ttu-id="93dd0-111">説明</span><span class="sxs-lookup"><span data-stu-id="93dd0-111">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="93dd0-112">[Get][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-112">[Get][]</span></span>                   | <span data-ttu-id="93dd0-113">lisItem</span><span class="sxs-lookup"><span data-stu-id="93dd0-113">lisItem</span></span>| <span data-ttu-id="93dd0-114">リスト内のアイテムを取得する。</span><span class="sxs-lookup"><span data-stu-id="93dd0-114">Get an item in a list</span></span>
| <span data-ttu-id="93dd0-115">[列の値 ][Get] を取得</span><span class="sxs-lookup"><span data-stu-id="93dd0-115">[Get column values][Get]</span></span>       | <span data-ttu-id="93dd0-116">listItem</span><span class="sxs-lookup"><span data-stu-id="93dd0-116">listItem</span></span> | <span data-ttu-id="93dd0-117">リスト アイテムから列の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-117">Get column values from listItem.</span></span>
| <span data-ttu-id="93dd0-118">[分析を取得する][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-118">[Get analytics][]</span></span>              | <span data-ttu-id="93dd0-119">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-119">[itemAnalytics][]</span></span>| <span data-ttu-id="93dd0-120">このリソースの分析を取得します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-120">Get analytics for this resource.</span></span> 
| <span data-ttu-id="93dd0-121">[間隔ごとにアクティビティを取得する][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-121">[Get activities by interval][]</span></span> | <span data-ttu-id="93dd0-122">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-122">[itemActivityStat][]</span></span>| <span data-ttu-id="93dd0-123">指定した時間間隔内に itemActivityStats のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-123">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="93dd0-124">[作成する][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-124">[Create][]</span></span>                     | <span data-ttu-id="93dd0-125">listItem</span><span class="sxs-lookup"><span data-stu-id="93dd0-125">listItem</span></span> | <span data-ttu-id="93dd0-126">リストに新しい listItem を作成します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-126">Create a new listItem in a list.</span></span>
| <span data-ttu-id="93dd0-127">[削除][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-127">[Delete][]</span></span>                     | <span data-ttu-id="93dd0-128">コンテンツはありません</span><span class="sxs-lookup"><span data-stu-id="93dd0-128">No Content</span></span> | <span data-ttu-id="93dd0-129">リストからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-129">Removes an item from a list.</span></span>
| <span data-ttu-id="93dd0-130">[更新][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-130">[Update][]</span></span>                     | <span data-ttu-id="93dd0-131">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-131">[fieldValueSet][]</span></span>| <span data-ttu-id="93dd0-132">リストアイテム のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-132">Update the properties on a listItem.</span></span>
| <span data-ttu-id="93dd0-133">[列の値 ][更新]を更新する</span><span class="sxs-lookup"><span data-stu-id="93dd0-133">[Update column values][Update]</span></span> | <span data-ttu-id="93dd0-134">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-134">[fieldValueSet][]</span></span>| <span data-ttu-id="93dd0-135">リスト アイテムの列の値を更新します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-135">Update column values on a listItem.</span></span>

[取得]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[分析を取得する]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[間隔によりアクティビティを取得する]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[Create]: ../api/listitem-create.md
[削除]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a><span data-ttu-id="93dd0-144">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93dd0-144">Properties</span></span>

<span data-ttu-id="93dd0-145">**listItem** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="93dd0-145">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="93dd0-146">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="93dd0-146">Property name</span></span> | <span data-ttu-id="93dd0-147">種類</span><span class="sxs-lookup"><span data-stu-id="93dd0-147">Type</span></span>                | <span data-ttu-id="93dd0-148">説明</span><span class="sxs-lookup"><span data-stu-id="93dd0-148">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="93dd0-149">contentType</span><span class="sxs-lookup"><span data-stu-id="93dd0-149">contentType</span></span>   | <span data-ttu-id="93dd0-150">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-150">[contentTypeInfo][]</span></span> | <span data-ttu-id="93dd0-151">このリスト アイテムのコンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="93dd0-151">The content type of this list item</span></span>

<span data-ttu-id="93dd0-152">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="93dd0-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="93dd0-153">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="93dd0-153">Property name</span></span>        | <span data-ttu-id="93dd0-154">種類</span><span class="sxs-lookup"><span data-stu-id="93dd0-154">Type</span></span>              | <span data-ttu-id="93dd0-155">説明</span><span class="sxs-lookup"><span data-stu-id="93dd0-155">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="93dd0-156">id</span><span class="sxs-lookup"><span data-stu-id="93dd0-156">id</span></span>                   | <span data-ttu-id="93dd0-157">string</span><span class="sxs-lookup"><span data-stu-id="93dd0-157">string</span></span>            | <span data-ttu-id="93dd0-p103">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="93dd0-160">name</span><span class="sxs-lookup"><span data-stu-id="93dd0-160">name</span></span>                 | <span data-ttu-id="93dd0-161">string</span><span class="sxs-lookup"><span data-stu-id="93dd0-161">string</span></span>            | <span data-ttu-id="93dd0-162">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="93dd0-162">The name / title of the item.</span></span>
| <span data-ttu-id="93dd0-163">createdBy</span><span class="sxs-lookup"><span data-stu-id="93dd0-163">createdBy</span></span>            | <span data-ttu-id="93dd0-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-164">[identitySet][]</span></span>   | <span data-ttu-id="93dd0-165">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-165">Identity of the creator of this item.</span></span> <span data-ttu-id="93dd0-166">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-166">Read-only.</span></span>
| <span data-ttu-id="93dd0-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93dd0-167">createdDateTime</span></span>      | <span data-ttu-id="93dd0-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93dd0-168">DateTimeOffset</span></span>    | <span data-ttu-id="93dd0-p105">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="93dd0-171">description</span><span class="sxs-lookup"><span data-stu-id="93dd0-171">description</span></span>          | <span data-ttu-id="93dd0-172">string</span><span class="sxs-lookup"><span data-stu-id="93dd0-172">string</span></span>            | <span data-ttu-id="93dd0-173">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="93dd0-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="93dd0-174">eTag</span><span class="sxs-lookup"><span data-stu-id="93dd0-174">eTag</span></span>                 | <span data-ttu-id="93dd0-175">string</span><span class="sxs-lookup"><span data-stu-id="93dd0-175">string</span></span>            | <span data-ttu-id="93dd0-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="93dd0-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="93dd0-178">lastModifiedBy</span></span>       | <span data-ttu-id="93dd0-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-179">[identitySet][]</span></span>   | <span data-ttu-id="93dd0-180">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="93dd0-181">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-181">Read-only.</span></span>
| <span data-ttu-id="93dd0-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93dd0-182">lastModifiedDateTime</span></span> | <span data-ttu-id="93dd0-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93dd0-183">DateTimeOffset</span></span>    | <span data-ttu-id="93dd0-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="93dd0-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="93dd0-186">parentReference</span></span>      | <span data-ttu-id="93dd0-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-187">[itemReference][]</span></span> | <span data-ttu-id="93dd0-p109">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="93dd0-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="93dd0-190">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="93dd0-190">sharepointIds</span></span>        | <span data-ttu-id="93dd0-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-191">[sharepointIds][]</span></span> | <span data-ttu-id="93dd0-p110">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="93dd0-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="93dd0-194">webUrl</span></span>               | <span data-ttu-id="93dd0-195">string (URL)</span><span class="sxs-lookup"><span data-stu-id="93dd0-195">string (url)</span></span>      | <span data-ttu-id="93dd0-p111">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="93dd0-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93dd0-198">Relationships</span></span>

 <span data-ttu-id="93dd0-199">**listItem** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="93dd0-199">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="93dd0-200">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="93dd0-200">Relationship name</span></span> | <span data-ttu-id="93dd0-201">種類</span><span class="sxs-lookup"><span data-stu-id="93dd0-201">Type</span></span>                           | <span data-ttu-id="93dd0-202">説明</span><span class="sxs-lookup"><span data-stu-id="93dd0-202">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="93dd0-203">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="93dd0-203">activities</span></span>        | <span data-ttu-id="93dd0-204">[itemActivity][] コレクション</span><span class="sxs-lookup"><span data-stu-id="93dd0-204">[itemActivity][] collection</span></span>    | <span data-ttu-id="93dd0-205">このアイテムに対して行われた最近のアクティビティのリストです。</span><span class="sxs-lookup"><span data-stu-id="93dd0-205">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="93dd0-206">分析</span><span class="sxs-lookup"><span data-stu-id="93dd0-206">analytics</span></span>         | <span data-ttu-id="93dd0-207">[itemAnalytics][] リソース</span><span class="sxs-lookup"><span data-stu-id="93dd0-207">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="93dd0-208">このアイテムについて行われたビュー アクティビティに関する分析。</span><span class="sxs-lookup"><span data-stu-id="93dd0-208">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="93dd0-209">driveItem</span><span class="sxs-lookup"><span data-stu-id="93dd0-209">driveItem</span></span>         | <span data-ttu-id="93dd0-210">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-210">[driveItem][]</span></span>                  | <span data-ttu-id="93dd0-211">ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。</span><span class="sxs-lookup"><span data-stu-id="93dd0-211">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="93dd0-212">フィールド</span><span class="sxs-lookup"><span data-stu-id="93dd0-212">fields</span></span>            | <span data-ttu-id="93dd0-213">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="93dd0-213">[fieldValueSet][]</span></span>              | <span data-ttu-id="93dd0-214">このリスト アイテムの列セットの値です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-214">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="93dd0-215">versions</span><span class="sxs-lookup"><span data-stu-id="93dd0-215">versions</span></span>          | <span data-ttu-id="93dd0-216">[listItemVersion][] コレクション</span><span class="sxs-lookup"><span data-stu-id="93dd0-216">[listItemVersion][] collection</span></span> | <span data-ttu-id="93dd0-217">リスト アイテムの以前のバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="93dd0-217">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="93dd0-229">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93dd0-229">JSON representation</span></span>

<span data-ttu-id="93dd0-230">以下は、**listItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="93dd0-230">Here is a JSON representation of a **listItem** resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/listItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
