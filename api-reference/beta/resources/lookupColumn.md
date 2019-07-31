---
author: JeremyKelley
description: columnDefinition リソースの lookupColumn は、列の値がサイト内の別のソースから検索されることを示します。
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8c92bce6b6d7ba401f6b9274f2ba0eee4439929e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009910"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="04177-103">LookupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04177-103">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04177-104">[columnDefinition](columndefinition.md) リソースの **lookupColumn** は、列の値がサイト内の別のソースから検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="04177-104">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04177-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04177-105">JSON representation</span></span>

<span data-ttu-id="04177-106">以下は、**lookupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04177-106">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="04177-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04177-107">Properties</span></span>

| <span data-ttu-id="04177-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="04177-108">Property name</span></span>             | <span data-ttu-id="04177-109">種類</span><span class="sxs-lookup"><span data-stu-id="04177-109">Type</span></span>    | <span data-ttu-id="04177-110">説明</span><span class="sxs-lookup"><span data-stu-id="04177-110">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="04177-111">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="04177-111">**allowMultipleValues**</span></span>   | <span data-ttu-id="04177-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="04177-112">boolean</span></span> | <span data-ttu-id="04177-113">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="04177-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="04177-114">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="04177-114">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="04177-115">boolean</span><span class="sxs-lookup"><span data-stu-id="04177-115">boolean</span></span> | <span data-ttu-id="04177-116">列の値が標準の 255 文字の制限を超えることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="04177-116">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="04177-117">**columnName**</span><span class="sxs-lookup"><span data-stu-id="04177-117">**columnName**</span></span>            | <span data-ttu-id="04177-118">string</span><span class="sxs-lookup"><span data-stu-id="04177-118">string</span></span>  | <span data-ttu-id="04177-119">検索元の列の名前。</span><span class="sxs-lookup"><span data-stu-id="04177-119">The name of the lookup source column.</span></span>
| <span data-ttu-id="04177-120">**listId**</span><span class="sxs-lookup"><span data-stu-id="04177-120">**listId**</span></span>                | <span data-ttu-id="04177-121">string</span><span class="sxs-lookup"><span data-stu-id="04177-121">string</span></span>  | <span data-ttu-id="04177-122">検索元リストの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="04177-122">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="04177-123">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="04177-123">**primaryLookupColumnId**</span></span> | <span data-ttu-id="04177-124">string</span><span class="sxs-lookup"><span data-stu-id="04177-124">string</span></span>  | <span data-ttu-id="04177-125">指定されている場合、この列は*セカンダリ ルックアップ*であり、*プライマリ ルックアップ*によって検索されたリスト項目から、新たに追加されたフィールドを取り出します。</span><span class="sxs-lookup"><span data-stu-id="04177-125">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="04177-126">*プライマリ*によって検索されたリスト項目を、ここで指定された列のソースとして使用します。</span><span class="sxs-lookup"><span data-stu-id="04177-126">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": []
}
-->
