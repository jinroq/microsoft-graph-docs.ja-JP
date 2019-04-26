---
title: educationCategory リソースの種類
description: 割り当てに適用できるカテゴリ。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bf5ee33ec7d217c0bc4c6e4d35666d6e9f34dadb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340602"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="8104d-103">educationCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8104d-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8104d-104">割り当てに適用できるカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="8104d-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="8104d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="8104d-105">Methods</span></span>

| <span data-ttu-id="8104d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8104d-106">Method</span></span>           | <span data-ttu-id="8104d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8104d-107">Return Type</span></span>    |<span data-ttu-id="8104d-108">説明</span><span class="sxs-lookup"><span data-stu-id="8104d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8104d-109">educationCategory を取得する</span><span class="sxs-lookup"><span data-stu-id="8104d-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="8104d-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="8104d-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="8104d-111">既存の**educationCategory**を取得します。</span><span class="sxs-lookup"><span data-stu-id="8104d-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="8104d-112">カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="8104d-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="8104d-113">なし</span><span class="sxs-lookup"><span data-stu-id="8104d-113">None</span></span> | <span data-ttu-id="8104d-114">**educationCategory**を削除します。</span><span class="sxs-lookup"><span data-stu-id="8104d-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="8104d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8104d-115">Properties</span></span>
| <span data-ttu-id="8104d-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8104d-116">Property</span></span>     | <span data-ttu-id="8104d-117">型</span><span class="sxs-lookup"><span data-stu-id="8104d-117">Type</span></span>   |<span data-ttu-id="8104d-118">説明</span><span class="sxs-lookup"><span data-stu-id="8104d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8104d-119">id</span><span class="sxs-lookup"><span data-stu-id="8104d-119">id</span></span>|<span data-ttu-id="8104d-120">String</span><span class="sxs-lookup"><span data-stu-id="8104d-120">String</span></span>|<span data-ttu-id="8104d-121">カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="8104d-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="8104d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="8104d-122">displayName</span></span>|<span data-ttu-id="8104d-123">String</span><span class="sxs-lookup"><span data-stu-id="8104d-123">String</span></span>|<span data-ttu-id="8104d-124">カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="8104d-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8104d-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8104d-125">JSON representation</span></span>

<span data-ttu-id="8104d-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8104d-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
