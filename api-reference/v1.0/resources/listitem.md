---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: 13ddb00d90880570361c7dcbe198c7c90e044957
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264400"
---
# <a name="listitem-resource"></a><span data-ttu-id="59e44-102">ListItem リソース</span><span class="sxs-lookup"><span data-stu-id="59e44-102">ListItem resource</span></span>

<span data-ttu-id="59e44-103">このリソースは、SharePoint の **[list][]** 内のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="59e44-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="59e44-104">リスト内の列の値は、`fieldValueSet` ディクショナリから利用できます。</span><span class="sxs-lookup"><span data-stu-id="59e44-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="59e44-105">listItem に関するタスク</span><span class="sxs-lookup"><span data-stu-id="59e44-105">Tasks on a listItem</span></span>

<span data-ttu-id="59e44-106">**listItem** リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="59e44-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="59e44-107">以下のすべての例は、`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}` などの**[list][]** からの相対指定です。</span><span class="sxs-lookup"><span data-stu-id="59e44-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="59e44-108">共通タスク</span><span class="sxs-lookup"><span data-stu-id="59e44-108">Common task</span></span>                    | <span data-ttu-id="59e44-109">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="59e44-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="59e44-110">[取得][]</span><span class="sxs-lookup"><span data-stu-id="59e44-110">[Get][]</span></span>                        | <span data-ttu-id="59e44-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="59e44-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="59e44-112">[列の値の取得][取得]</span><span class="sxs-lookup"><span data-stu-id="59e44-112">[Get column values][Get]</span></span>       | <span data-ttu-id="59e44-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="59e44-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="59e44-114">[作成][]</span><span class="sxs-lookup"><span data-stu-id="59e44-114">[Create][]</span></span>                     | <span data-ttu-id="59e44-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="59e44-115">POST /items</span></span>
| <span data-ttu-id="59e44-116">[削除][]</span><span class="sxs-lookup"><span data-stu-id="59e44-116">[Delete][]</span></span>                     | <span data-ttu-id="59e44-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="59e44-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="59e44-118">[更新][]</span><span class="sxs-lookup"><span data-stu-id="59e44-118">[Update][]</span></span>                     | <span data-ttu-id="59e44-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="59e44-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="59e44-120">[列の値の更新][更新]</span><span class="sxs-lookup"><span data-stu-id="59e44-120">[Update column values][Update]</span></span> | <span data-ttu-id="59e44-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="59e44-121">PATCH /items/{item-id}/fields</span></span>

[取得]: ../api/listItem_get.md
[Get]: ../api/listItem_get.md
[作成]: ../api/listItem_create.md
[Create]: ../api/listItem_create.md
[削除]: ../api/listItem_delete.md
[Delete]: ../api/listItem_delete.md
[更新]: ../api/listItem_update.md
[Update]: ../api/listItem_update.md

## <a name="json-representation"></a><span data-ttu-id="59e44-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59e44-126">JSON representation</span></span>

<span data-ttu-id="59e44-127">以下は、**listItem** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59e44-127">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="59e44-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59e44-128">Properties</span></span>

<span data-ttu-id="59e44-129">**listItem** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="59e44-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="59e44-130">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="59e44-130">Property name</span></span> | <span data-ttu-id="59e44-131">型</span><span class="sxs-lookup"><span data-stu-id="59e44-131">Type</span></span>                | <span data-ttu-id="59e44-132">説明</span><span class="sxs-lookup"><span data-stu-id="59e44-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="59e44-133">contentType</span><span class="sxs-lookup"><span data-stu-id="59e44-133">contentType</span></span>   | <span data-ttu-id="59e44-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="59e44-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="59e44-135">このリスト アイテムのコンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="59e44-135">The content type of this list item</span></span>

<span data-ttu-id="59e44-136">次のプロパティは、**[baseItem][]** から継承しています。</span><span class="sxs-lookup"><span data-stu-id="59e44-136">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="59e44-137">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="59e44-137">Property name</span></span>        | <span data-ttu-id="59e44-138">型</span><span class="sxs-lookup"><span data-stu-id="59e44-138">Type</span></span>              | <span data-ttu-id="59e44-139">説明</span><span class="sxs-lookup"><span data-stu-id="59e44-139">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="59e44-140">ID</span><span class="sxs-lookup"><span data-stu-id="59e44-140">id</span></span>                   | <span data-ttu-id="59e44-141">文字列</span><span class="sxs-lookup"><span data-stu-id="59e44-141">string</span></span>            | <span data-ttu-id="59e44-p103">アイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e44-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="59e44-144">名前</span><span class="sxs-lookup"><span data-stu-id="59e44-144">name</span></span>                 | <span data-ttu-id="59e44-145">文字列</span><span class="sxs-lookup"><span data-stu-id="59e44-145">string</span></span>            | <span data-ttu-id="59e44-146">アイテムの名前/タイトル。</span><span class="sxs-lookup"><span data-stu-id="59e44-146">The name / title of the item.</span></span>
| <span data-ttu-id="59e44-147">createdBy</span><span class="sxs-lookup"><span data-stu-id="59e44-147">createdBy</span></span>            | <span data-ttu-id="59e44-148">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="59e44-148">[identitySet][]</span></span>   | <span data-ttu-id="59e44-149">このアイテムの作成者の ID です。</span><span class="sxs-lookup"><span data-stu-id="59e44-149">Identity of the creator of this item.</span></span> <span data-ttu-id="59e44-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e44-150">Read-only.</span></span>
| <span data-ttu-id="59e44-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59e44-151">createdDateTime</span></span>      | <span data-ttu-id="59e44-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59e44-152">DateTimeOffset</span></span>    | <span data-ttu-id="59e44-p105">アイテムが作成された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e44-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="59e44-155">説明</span><span class="sxs-lookup"><span data-stu-id="59e44-155">description</span></span>          | <span data-ttu-id="59e44-156">文字列</span><span class="sxs-lookup"><span data-stu-id="59e44-156">string</span></span>            | <span data-ttu-id="59e44-157">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="59e44-157">The descriptive text for the item.</span></span>
| <span data-ttu-id="59e44-158">eTag</span><span class="sxs-lookup"><span data-stu-id="59e44-158">eTag</span></span>                 | <span data-ttu-id="59e44-159">文字列</span><span class="sxs-lookup"><span data-stu-id="59e44-159">string</span></span>            | <span data-ttu-id="59e44-p106">アイテムの ETag。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e44-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="59e44-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="59e44-162">lastModifiedBy</span></span>       | <span data-ttu-id="59e44-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="59e44-163">[identitySet][]</span></span>   | <span data-ttu-id="59e44-164">このアイテムの最終変更者の ID です。</span><span class="sxs-lookup"><span data-stu-id="59e44-164">Identity of the last modifier of this item.</span></span> <span data-ttu-id="59e44-165">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e44-165">Read-only.</span></span>
| <span data-ttu-id="59e44-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59e44-166">lastModifiedDateTime</span></span> | <span data-ttu-id="59e44-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59e44-167">DateTimeOffset</span></span>    | <span data-ttu-id="59e44-p108">アイテムが最後に変更された日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e44-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="59e44-170">parentReference</span><span class="sxs-lookup"><span data-stu-id="59e44-170">parentReference</span></span>      | <span data-ttu-id="59e44-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="59e44-171">[itemReference][]</span></span> | <span data-ttu-id="59e44-p109">親の情報 (アイテムに親がある場合)。読み取り/書き込み。</span><span class="sxs-lookup"><span data-stu-id="59e44-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="59e44-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="59e44-174">sharepointIds</span></span>        | <span data-ttu-id="59e44-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="59e44-175">[sharepointIds][]</span></span> | <span data-ttu-id="59e44-p110">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e44-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="59e44-178">webUrl</span><span class="sxs-lookup"><span data-stu-id="59e44-178">webUrl</span></span>               | <span data-ttu-id="59e44-179">string (URL)</span><span class="sxs-lookup"><span data-stu-id="59e44-179">string (url)</span></span>      | <span data-ttu-id="59e44-p111">ブラウザーでアイテムを表示する URL。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="59e44-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="59e44-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="59e44-182">Relationships</span></span>

 <span data-ttu-id="59e44-183">**listItem** リソースには、他のリソースと次のような関係があります。</span><span class="sxs-lookup"><span data-stu-id="59e44-183">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="59e44-184">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="59e44-184">Relationship name</span></span> | <span data-ttu-id="59e44-185">種類</span><span class="sxs-lookup"><span data-stu-id="59e44-185">Type</span></span>                           | <span data-ttu-id="59e44-186">説明</span><span class="sxs-lookup"><span data-stu-id="59e44-186">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="59e44-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="59e44-187">driveItem</span></span>         | <span data-ttu-id="59e44-188">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="59e44-188">[driveItem][]</span></span>                  | <span data-ttu-id="59e44-189">ドキュメント ライブラリの場合、**driveItem** リレーションシップは listItem を **[driveItem][]** として公開します。</span><span class="sxs-lookup"><span data-stu-id="59e44-189">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="59e44-190">フィールド</span><span class="sxs-lookup"><span data-stu-id="59e44-190">fields</span></span>            | <span data-ttu-id="59e44-191">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="59e44-191">[fieldValueSet][]</span></span>              | <span data-ttu-id="59e44-192">このリスト アイテムの列セットの値です。</span><span class="sxs-lookup"><span data-stu-id="59e44-192">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="59e44-193">バージョン</span><span class="sxs-lookup"><span data-stu-id="59e44-193">versions</span></span>          | <span data-ttu-id="59e44-194">[listItemVersion][] コレクション</span><span class="sxs-lookup"><span data-stu-id="59e44-194">[listItemVersion][] collection</span></span> | <span data-ttu-id="59e44-195">リスト項目の以前のバージョンの一覧です。</span><span class="sxs-lookup"><span data-stu-id="59e44-195">The list of previous versions of the list item.</span></span>

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[itemReference]: itemreference.md
[リスト]: list.md
[list]: list.md
[listItemVersion]: listItemVersion.md
[sharepointIds]: sharepointIds.md

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
