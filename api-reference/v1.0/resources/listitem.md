---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: eabb88eb6ad2eee7a032b2486555aa26c557ba1a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="listitem-resource"></a><span data-ttu-id="f90cb-102">ListItem リソース</span><span class="sxs-lookup"><span data-stu-id="f90cb-102">ListItem resource</span></span>

<span data-ttu-id="f90cb-103">このリソースは、SharePoint の **[list][]** 内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f90cb-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="f90cb-104">リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。</span><span class="sxs-lookup"><span data-stu-id="f90cb-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="f90cb-105">listItem に関するタスク</span><span class="sxs-lookup"><span data-stu-id="f90cb-105">Tasks on a listItem</span></span>

<span data-ttu-id="f90cb-106">**listItem** リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="f90cb-106">The following tasks are available for {type} resources.</span></span>
<span data-ttu-id="f90cb-107">以下のすべての例は、`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}` などの**[list][]** からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="f90cb-108">共通タスク</span><span class="sxs-lookup"><span data-stu-id="f90cb-108">Common task</span></span>                    | <span data-ttu-id="f90cb-109">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="f90cb-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="f90cb-110">[取得][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-110">[Get][]</span></span>                        | <span data-ttu-id="f90cb-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f90cb-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="f90cb-112">[列の値の取得][取得]</span><span class="sxs-lookup"><span data-stu-id="f90cb-112">[Get column values][Get]</span></span>       | <span data-ttu-id="f90cb-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="f90cb-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="f90cb-114">[作成][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-114">[Create][]</span></span>                     | <span data-ttu-id="f90cb-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="f90cb-115">Post items</span></span>
| <span data-ttu-id="f90cb-116">[削除][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-116">[Delete][]</span></span>                     | <span data-ttu-id="f90cb-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f90cb-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="f90cb-118">[更新][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-118">[Update][]</span></span>                     | <span data-ttu-id="f90cb-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="f90cb-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="f90cb-120">[列の値の更新][更新]</span><span class="sxs-lookup"><span data-stu-id="f90cb-120">[Update column values][Update]</span></span> | <span data-ttu-id="f90cb-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="f90cb-121">PATCH /items/{item-id}/fields</span></span>

[取得]: ../api/listItem_get.md
[作成]: ../api/listItem_create.md
[削除]: ../api/listItem_delete.md
[更新]: ../api/listItem_update.md

## <a name="json-representation"></a><span data-ttu-id="f90cb-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f90cb-126">JSON representation</span></span>

<span data-ttu-id="f90cb-127">以下は、**listItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-127">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="f90cb-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f90cb-128">Properties</span></span>

<span data-ttu-id="f90cb-129">**listItem** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="f90cb-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="f90cb-130">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f90cb-130">Property name</span></span> | <span data-ttu-id="f90cb-131">種類</span><span class="sxs-lookup"><span data-stu-id="f90cb-131">Type</span></span>                | <span data-ttu-id="f90cb-132">説明</span><span class="sxs-lookup"><span data-stu-id="f90cb-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="f90cb-133">contentType</span><span class="sxs-lookup"><span data-stu-id="f90cb-133">contentType</span></span>   | <span data-ttu-id="f90cb-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="f90cb-135">このリスト アイテムのコンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="f90cb-135">The content type of this list item</span></span>
| <span data-ttu-id="f90cb-136">fields</span><span class="sxs-lookup"><span data-stu-id="f90cb-136">fields</span></span>        | <span data-ttu-id="f90cb-137">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-137">[fieldValueSet][]</span></span>   | <span data-ttu-id="f90cb-138">このリスト アイテムの列セットの値です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-138">The values of the columns set on this list item.</span></span>

<span data-ttu-id="f90cb-139">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="f90cb-139">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="f90cb-140">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f90cb-140">Property name</span></span>        | <span data-ttu-id="f90cb-141">種類</span><span class="sxs-lookup"><span data-stu-id="f90cb-141">Type</span></span>             | <span data-ttu-id="f90cb-142">説明</span><span class="sxs-lookup"><span data-stu-id="f90cb-142">Description</span></span>
|:---------------------|:-----------------|:-----------------------------------
| <span data-ttu-id="f90cb-143">id</span><span class="sxs-lookup"><span data-stu-id="f90cb-143">id</span></span>                   | <span data-ttu-id="f90cb-144">string</span><span class="sxs-lookup"><span data-stu-id="f90cb-144">string</span></span>           | <span data-ttu-id="f90cb-p103">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f90cb-147">name</span><span class="sxs-lookup"><span data-stu-id="f90cb-147">name</span></span>                 | <span data-ttu-id="f90cb-148">string</span><span class="sxs-lookup"><span data-stu-id="f90cb-148">string</span></span>           | <span data-ttu-id="f90cb-149">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="f90cb-149">The name / title of the item.</span></span>
| <span data-ttu-id="f90cb-150">createdBy</span><span class="sxs-lookup"><span data-stu-id="f90cb-150">createdBy</span></span>            | <span data-ttu-id="f90cb-151">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-151">[identitySet][]</span></span>  | <span data-ttu-id="f90cb-152">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-152">Identity of the creator of this item.</span></span> <span data-ttu-id="f90cb-153">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-153">Read-only.</span></span>
| <span data-ttu-id="f90cb-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f90cb-154">createdDateTime</span></span>      | <span data-ttu-id="f90cb-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f90cb-155">DateTimeOffset</span></span>   | <span data-ttu-id="f90cb-p105">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f90cb-158">description</span><span class="sxs-lookup"><span data-stu-id="f90cb-158">description</span></span>          | <span data-ttu-id="f90cb-159">string</span><span class="sxs-lookup"><span data-stu-id="f90cb-159">string</span></span>           | <span data-ttu-id="f90cb-160">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="f90cb-160">The descriptive text for the site.</span></span>
| <span data-ttu-id="f90cb-161">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f90cb-161">lastModifiedBy</span></span>       | <span data-ttu-id="f90cb-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-162">[identitySet][]</span></span>  | <span data-ttu-id="f90cb-163">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-163">Identity of the last modifier of this item.</span></span> <span data-ttu-id="f90cb-164">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-164">Read-only.</span></span>
| <span data-ttu-id="f90cb-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f90cb-165">lastModifiedDateTime</span></span> | <span data-ttu-id="f90cb-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f90cb-166">DateTimeOffset</span></span>   | <span data-ttu-id="f90cb-p107">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f90cb-169">webUrl</span><span class="sxs-lookup"><span data-stu-id="f90cb-169">webUrl</span></span>               | <span data-ttu-id="f90cb-170">string (URL)</span><span class="sxs-lookup"><span data-stu-id="f90cb-170">string (url)</span></span>     | <span data-ttu-id="f90cb-p108">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f90cb-p108">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f90cb-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f90cb-173">Relationships</span></span>

 <span data-ttu-id="f90cb-174">**listItem** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="f90cb-174">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="f90cb-175">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="f90cb-175">Relationship name</span></span> | <span data-ttu-id="f90cb-176">種類</span><span class="sxs-lookup"><span data-stu-id="f90cb-176">Type</span></span>                        | <span data-ttu-id="f90cb-177">説明</span><span class="sxs-lookup"><span data-stu-id="f90cb-177">Description</span></span>
|:------------------|:----------------------------|:-------------------------------
| <span data-ttu-id="f90cb-178">driveItem</span><span class="sxs-lookup"><span data-stu-id="f90cb-178">driveItem</span></span>         | <span data-ttu-id="f90cb-179">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="f90cb-179">[driveItem][]</span></span>               | <span data-ttu-id="f90cb-180">ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。</span><span class="sxs-lookup"><span data-stu-id="f90cb-180">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

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
