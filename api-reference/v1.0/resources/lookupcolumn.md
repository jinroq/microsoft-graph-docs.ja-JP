---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 73d372d52447906c826d79e3c614635a3023cefa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022835"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="75297-102">LookupColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75297-102">LookupColumn resource type</span></span>

<span data-ttu-id="75297-103">[columnDefinition](columndefinition.md) リソースの **lookupColumn** は、列の値がサイト内の別のソースから検索されることを示します。</span><span class="sxs-lookup"><span data-stu-id="75297-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="75297-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75297-104">JSON representation</span></span>

<span data-ttu-id="75297-105">以下は、**lookupColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75297-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="75297-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75297-106">Properties</span></span>

| <span data-ttu-id="75297-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="75297-107">Property name</span></span>             | <span data-ttu-id="75297-108">種類</span><span class="sxs-lookup"><span data-stu-id="75297-108">Type</span></span>    | <span data-ttu-id="75297-109">説明</span><span class="sxs-lookup"><span data-stu-id="75297-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="75297-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="75297-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="75297-111">boolean</span><span class="sxs-lookup"><span data-stu-id="75297-111">boolean</span></span> | <span data-ttu-id="75297-112">ソースから複数の値を選択できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="75297-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="75297-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="75297-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="75297-114">boolean</span><span class="sxs-lookup"><span data-stu-id="75297-114">boolean</span></span> | <span data-ttu-id="75297-115">列の値が標準の 255 文字の制限を超えることができるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="75297-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="75297-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="75297-116">**columnName**</span></span>            | <span data-ttu-id="75297-117">string</span><span class="sxs-lookup"><span data-stu-id="75297-117">string</span></span>  | <span data-ttu-id="75297-118">検索元の列の名前。</span><span class="sxs-lookup"><span data-stu-id="75297-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="75297-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="75297-119">**listId**</span></span>                | <span data-ttu-id="75297-120">string</span><span class="sxs-lookup"><span data-stu-id="75297-120">string</span></span>  | <span data-ttu-id="75297-121">検索元リストの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="75297-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="75297-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="75297-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="75297-123">string</span><span class="sxs-lookup"><span data-stu-id="75297-123">string</span></span>  | <span data-ttu-id="75297-124">指定されている場合、この列は*セカンダリ ルックアップ*であり、*プライマリ ルックアップ*によって検索されたリスト項目から、新たに追加されたフィールドを取り出します。</span><span class="sxs-lookup"><span data-stu-id="75297-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="75297-125">*プライマリ*によって検索されたリスト項目を、ここで指定された列のソースとして使用します。</span><span class="sxs-lookup"><span data-stu-id="75297-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
