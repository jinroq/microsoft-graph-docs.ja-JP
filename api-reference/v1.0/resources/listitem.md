---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
localization_priority: Priority
ms.openlocfilehash: bee264fb46e08d55893f41ae6be2a64edb06c3fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833027"
---
# <a name="listitem-resource"></a><span data-ttu-id="0daa3-102">ListItem リソース</span><span class="sxs-lookup"><span data-stu-id="0daa3-102">ListItem resource</span></span>

<span data-ttu-id="0daa3-103">このリソースは、SharePoint の **[list][]** 内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0daa3-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="0daa3-104">リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。</span><span class="sxs-lookup"><span data-stu-id="0daa3-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="0daa3-105">listItem に関するタスク</span><span class="sxs-lookup"><span data-stu-id="0daa3-105">Tasks on a listItem</span></span>

<span data-ttu-id="0daa3-106">**listItem** リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="0daa3-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="0daa3-107">以下のすべての例は、`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}` などの**[list][]** からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="0daa3-108">共通タスク</span><span class="sxs-lookup"><span data-stu-id="0daa3-108">Common task</span></span>                    | <span data-ttu-id="0daa3-109">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="0daa3-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="0daa3-110">[取得][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-110">[Get][]</span></span>                        | <span data-ttu-id="0daa3-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="0daa3-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="0daa3-112">[列の値の取得][取得]</span><span class="sxs-lookup"><span data-stu-id="0daa3-112">[Get column values][Get]</span></span>       | <span data-ttu-id="0daa3-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="0daa3-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="0daa3-114">[作成][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-114">[Create][]</span></span>                     | <span data-ttu-id="0daa3-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="0daa3-115">POST /items</span></span>
| <span data-ttu-id="0daa3-116">[削除][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-116">[Delete][]</span></span>                     | <span data-ttu-id="0daa3-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="0daa3-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="0daa3-118">[更新][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-118">[Update][]</span></span>                     | <span data-ttu-id="0daa3-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="0daa3-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="0daa3-120">[列の値の更新][更新]</span><span class="sxs-lookup"><span data-stu-id="0daa3-120">[Update column values][Update]</span></span> | <span data-ttu-id="0daa3-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="0daa3-121">PATCH /items/{item-id}/fields</span></span>

[取得]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[作成]: ../api/listitem-create.md
[Create]: ../api/listitem-create.md
[削除]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[更新]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="0daa3-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0daa3-126">JSON representation</span></span>

<span data-ttu-id="0daa3-127">以下は、**listItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-127">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0daa3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0daa3-128">Properties</span></span>

<span data-ttu-id="0daa3-129">**listItem** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="0daa3-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="0daa3-130">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0daa3-130">Property name</span></span> | <span data-ttu-id="0daa3-131">種類</span><span class="sxs-lookup"><span data-stu-id="0daa3-131">Type</span></span>                | <span data-ttu-id="0daa3-132">説明</span><span class="sxs-lookup"><span data-stu-id="0daa3-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="0daa3-133">contentType</span><span class="sxs-lookup"><span data-stu-id="0daa3-133">contentType</span></span>   | <span data-ttu-id="0daa3-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="0daa3-135">このリスト アイテムのコンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="0daa3-135">The content type of this list item</span></span>

<span data-ttu-id="0daa3-136">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="0daa3-136">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="0daa3-137">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0daa3-137">Property name</span></span>        | <span data-ttu-id="0daa3-138">Type</span><span class="sxs-lookup"><span data-stu-id="0daa3-138">Type</span></span>              | <span data-ttu-id="0daa3-139">説明</span><span class="sxs-lookup"><span data-stu-id="0daa3-139">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="0daa3-140">ID</span><span class="sxs-lookup"><span data-stu-id="0daa3-140">id</span></span>                   | <span data-ttu-id="0daa3-141">文字列</span><span class="sxs-lookup"><span data-stu-id="0daa3-141">string</span></span>            | <span data-ttu-id="0daa3-p103">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="0daa3-144">name</span><span class="sxs-lookup"><span data-stu-id="0daa3-144">name</span></span>                 | <span data-ttu-id="0daa3-145">文字列</span><span class="sxs-lookup"><span data-stu-id="0daa3-145">string</span></span>            | <span data-ttu-id="0daa3-146">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="0daa3-146">The name / title of the item.</span></span>
| <span data-ttu-id="0daa3-147">createdBy</span><span class="sxs-lookup"><span data-stu-id="0daa3-147">createdBy</span></span>            | <span data-ttu-id="0daa3-148">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-148">[identitySet][]</span></span>   | <span data-ttu-id="0daa3-149">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-149">Identity of the creator of this item.</span></span> <span data-ttu-id="0daa3-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-150">Read-only.</span></span>
| <span data-ttu-id="0daa3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0daa3-151">createdDateTime</span></span>      | <span data-ttu-id="0daa3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0daa3-152">DateTimeOffset</span></span>    | <span data-ttu-id="0daa3-p105">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="0daa3-155">description</span><span class="sxs-lookup"><span data-stu-id="0daa3-155">description</span></span>          | <span data-ttu-id="0daa3-156">文字列</span><span class="sxs-lookup"><span data-stu-id="0daa3-156">string</span></span>            | <span data-ttu-id="0daa3-157">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="0daa3-157">The descriptive text for the item.</span></span>
| <span data-ttu-id="0daa3-158">eTag</span><span class="sxs-lookup"><span data-stu-id="0daa3-158">eTag</span></span>                 | <span data-ttu-id="0daa3-159">string</span><span class="sxs-lookup"><span data-stu-id="0daa3-159">string</span></span>            | <span data-ttu-id="0daa3-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="0daa3-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0daa3-162">lastModifiedBy</span></span>       | <span data-ttu-id="0daa3-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-163">[identitySet][]</span></span>   | <span data-ttu-id="0daa3-164">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-164">Identity of the last modifier of this item.</span></span> <span data-ttu-id="0daa3-165">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-165">Read-only.</span></span>
| <span data-ttu-id="0daa3-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0daa3-166">lastModifiedDateTime</span></span> | <span data-ttu-id="0daa3-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0daa3-167">DateTimeOffset</span></span>    | <span data-ttu-id="0daa3-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="0daa3-170">parentReference</span><span class="sxs-lookup"><span data-stu-id="0daa3-170">parentReference</span></span>      | <span data-ttu-id="0daa3-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-171">[itemReference][]</span></span> | <span data-ttu-id="0daa3-p109">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="0daa3-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="0daa3-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="0daa3-174">sharepointIds</span></span>        | <span data-ttu-id="0daa3-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-175">[sharepointIds][]</span></span> | <span data-ttu-id="0daa3-p110">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="0daa3-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="0daa3-178">webUrl</span></span>               | <span data-ttu-id="0daa3-179">string (URL)</span><span class="sxs-lookup"><span data-stu-id="0daa3-179">string (url)</span></span>      | <span data-ttu-id="0daa3-p111">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="0daa3-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0daa3-182">Relationships</span></span>

 <span data-ttu-id="0daa3-183">**listItem** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="0daa3-183">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="0daa3-184">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="0daa3-184">Relationship name</span></span> | <span data-ttu-id="0daa3-185">種類</span><span class="sxs-lookup"><span data-stu-id="0daa3-185">Type</span></span>                           | <span data-ttu-id="0daa3-186">説明</span><span class="sxs-lookup"><span data-stu-id="0daa3-186">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="0daa3-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="0daa3-187">driveItem</span></span>         | <span data-ttu-id="0daa3-188">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-188">[driveItem][]</span></span>                  | <span data-ttu-id="0daa3-189">ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。</span><span class="sxs-lookup"><span data-stu-id="0daa3-189">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="0daa3-190">fields</span><span class="sxs-lookup"><span data-stu-id="0daa3-190">fields</span></span>            | <span data-ttu-id="0daa3-191">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="0daa3-191">[fieldValueSet][]</span></span>              | <span data-ttu-id="0daa3-192">このリスト アイテムの列セットの値です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-192">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="0daa3-193">versions</span><span class="sxs-lookup"><span data-stu-id="0daa3-193">versions</span></span>          | <span data-ttu-id="0daa3-194">[listItemVersion][]コレクション</span><span class="sxs-lookup"><span data-stu-id="0daa3-194">[listItemVersion][] collection</span></span> | <span data-ttu-id="0daa3-195">リスト項目の以前のバージョンの一覧です。</span><span class="sxs-lookup"><span data-stu-id="0daa3-195">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
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
