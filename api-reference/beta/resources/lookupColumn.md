---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 92eb43dad2ceca173fba79ad7d40f51f488a992c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066541"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="381f8-102">LookupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="381f8-102">LookupColumn resource type</span></span>

> <span data-ttu-id="381f8-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="381f8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="381f8-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="381f8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="381f8-105">[columnDefinition](columndefinition.md) リソースの **lookupColumn** は、列の値がサイト内の別のソースから検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="381f8-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="381f8-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="381f8-106">JSON representation</span></span>

<span data-ttu-id="381f8-107">以下は、**lookupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="381f8-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="381f8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="381f8-108">Properties</span></span>

| <span data-ttu-id="381f8-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="381f8-109">Property name</span></span>             | <span data-ttu-id="381f8-110">型</span><span class="sxs-lookup"><span data-stu-id="381f8-110">Type</span></span>    | <span data-ttu-id="381f8-111">説明</span><span class="sxs-lookup"><span data-stu-id="381f8-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="381f8-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="381f8-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="381f8-113">boolean</span><span class="sxs-lookup"><span data-stu-id="381f8-113">boolean</span></span> | <span data-ttu-id="381f8-114">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="381f8-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="381f8-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="381f8-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="381f8-116">boolean</span><span class="sxs-lookup"><span data-stu-id="381f8-116">boolean</span></span> | <span data-ttu-id="381f8-117">列の値が標準の 255 文字の制限を超えることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="381f8-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="381f8-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="381f8-118">**columnName**</span></span>            | <span data-ttu-id="381f8-119">文字列</span><span class="sxs-lookup"><span data-stu-id="381f8-119">string</span></span>  | <span data-ttu-id="381f8-120">検索元の列の名前。</span><span class="sxs-lookup"><span data-stu-id="381f8-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="381f8-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="381f8-121">**listId**</span></span>                | <span data-ttu-id="381f8-122">文字列</span><span class="sxs-lookup"><span data-stu-id="381f8-122">string</span></span>  | <span data-ttu-id="381f8-123">検索元リストの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="381f8-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="381f8-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="381f8-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="381f8-125">文字列</span><span class="sxs-lookup"><span data-stu-id="381f8-125">string</span></span>  | <span data-ttu-id="381f8-126">指定されている場合、この列は*セカンダリ ルックアップ*であり、*プライマリ ルックアップ*によって検索されたリスト項目から、新たに追加されたフィールドを取り出します。</span><span class="sxs-lookup"><span data-stu-id="381f8-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="381f8-127">*プライマリ*によって検索されたリスト項目を、ここで指定された列のソースとして使用します。</span><span class="sxs-lookup"><span data-stu-id="381f8-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
