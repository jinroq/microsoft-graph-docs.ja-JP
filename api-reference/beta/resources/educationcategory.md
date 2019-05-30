---
title: educationCategory リソースの種類
description: 割り当てに適用できるカテゴリ。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: dd9eccac3a1b6b1bdc3b0eca4c87b5e29e2135a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536177"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="654d4-103">educationCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="654d4-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="654d4-104">割り当てに適用できるカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="654d4-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="654d4-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="654d4-105">Methods</span></span>

| <span data-ttu-id="654d4-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="654d4-106">Method</span></span>           | <span data-ttu-id="654d4-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="654d4-107">Return Type</span></span>    |<span data-ttu-id="654d4-108">説明</span><span class="sxs-lookup"><span data-stu-id="654d4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="654d4-109">EducationCategory を取得する</span><span class="sxs-lookup"><span data-stu-id="654d4-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="654d4-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="654d4-110">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="654d4-111">既存の**educationCategory**を取得します。</span><span class="sxs-lookup"><span data-stu-id="654d4-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="654d4-112">カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="654d4-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="654d4-113">None</span><span class="sxs-lookup"><span data-stu-id="654d4-113">None</span></span> | <span data-ttu-id="654d4-114">**EducationCategory**を削除します。</span><span class="sxs-lookup"><span data-stu-id="654d4-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="654d4-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="654d4-115">Properties</span></span>
| <span data-ttu-id="654d4-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="654d4-116">Property</span></span>     | <span data-ttu-id="654d4-117">型</span><span class="sxs-lookup"><span data-stu-id="654d4-117">Type</span></span>   |<span data-ttu-id="654d4-118">説明</span><span class="sxs-lookup"><span data-stu-id="654d4-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="654d4-119">id</span><span class="sxs-lookup"><span data-stu-id="654d4-119">id</span></span>|<span data-ttu-id="654d4-120">文字列</span><span class="sxs-lookup"><span data-stu-id="654d4-120">String</span></span>|<span data-ttu-id="654d4-121">カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="654d4-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="654d4-122">displayName</span><span class="sxs-lookup"><span data-stu-id="654d4-122">displayName</span></span>|<span data-ttu-id="654d4-123">String</span><span class="sxs-lookup"><span data-stu-id="654d4-123">String</span></span>|<span data-ttu-id="654d4-124">カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="654d4-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="654d4-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="654d4-125">JSON representation</span></span>

<span data-ttu-id="654d4-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="654d4-126">The following is a JSON representation of the resource.</span></span>

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
