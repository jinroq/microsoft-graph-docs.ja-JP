---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 07dba3c223ffc3993be1fc284572810a7aa3ccf8
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="ee329-102">LookupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee329-102">LookupColumn resource type</span></span>

<span data-ttu-id="ee329-103">[columnDefinition](columnDefinition.md) リソースの **lookupColumn** は、列の値がサイト内の別のソースから検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="ee329-103">The **lookupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee329-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee329-104">JSON representation</span></span>

<span data-ttu-id="ee329-105">以下は、**lookupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ee329-105">Here is a JSON representation of a **driveItem** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="ee329-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee329-106">Properties</span></span>

| <span data-ttu-id="ee329-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ee329-107">Property name</span></span>             | <span data-ttu-id="ee329-108">種類</span><span class="sxs-lookup"><span data-stu-id="ee329-108">Type</span></span>    | <span data-ttu-id="ee329-109">説明</span><span class="sxs-lookup"><span data-stu-id="ee329-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="ee329-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="ee329-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="ee329-111">boolean</span><span class="sxs-lookup"><span data-stu-id="ee329-111">boolean</span></span> | <span data-ttu-id="ee329-112">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ee329-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="ee329-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="ee329-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="ee329-114">boolean</span><span class="sxs-lookup"><span data-stu-id="ee329-114">boolean</span></span> | <span data-ttu-id="ee329-115">列の値が標準の 255 文字の制限を超えることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ee329-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="ee329-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="ee329-116">**columnName**</span></span>            | <span data-ttu-id="ee329-117">string</span><span class="sxs-lookup"><span data-stu-id="ee329-117">string</span></span>  | <span data-ttu-id="ee329-118">検索元の列の名前。</span><span class="sxs-lookup"><span data-stu-id="ee329-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="ee329-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="ee329-119">**listId**</span></span>                | <span data-ttu-id="ee329-120">string</span><span class="sxs-lookup"><span data-stu-id="ee329-120">string</span></span>  | <span data-ttu-id="ee329-121">検索元リストの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ee329-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="ee329-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="ee329-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="ee329-123">string</span><span class="sxs-lookup"><span data-stu-id="ee329-123">string</span></span>  | <span data-ttu-id="ee329-124">指定されている場合、この列は*セカンダリ ルックアップ*であり、*プライマリ ルックアップ*によって検索されたリスト アイテムから、新たに追加されたフィールドを取り出します。</span><span class="sxs-lookup"><span data-stu-id="ee329-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="ee329-125">*プライマリ*によって検索されたリスト アイテムを、ここで指定された列のソースとして使用します。</span><span class="sxs-lookup"><span data-stu-id="ee329-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
