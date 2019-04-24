---
title: educationCategory リソースの種類
description: 割り当てに適用できるカテゴリ。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 928f37b4d29a4443c947bd92bf4a71f9f8a05f59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507318"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="0d54a-103">educationCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0d54a-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d54a-104">割り当てに適用できるカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="0d54a-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="0d54a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d54a-105">Methods</span></span>

| <span data-ttu-id="0d54a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0d54a-106">Method</span></span>           | <span data-ttu-id="0d54a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0d54a-107">Return Type</span></span>    |<span data-ttu-id="0d54a-108">説明</span><span class="sxs-lookup"><span data-stu-id="0d54a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d54a-109">educationCategory を取得する</span><span class="sxs-lookup"><span data-stu-id="0d54a-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="0d54a-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="0d54a-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="0d54a-111">既存の**educationCategory**を取得します。</span><span class="sxs-lookup"><span data-stu-id="0d54a-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="0d54a-112">カテゴリを削除する</span><span class="sxs-lookup"><span data-stu-id="0d54a-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="0d54a-113">なし</span><span class="sxs-lookup"><span data-stu-id="0d54a-113">None</span></span> | <span data-ttu-id="0d54a-114">**educationCategory**を削除します。</span><span class="sxs-lookup"><span data-stu-id="0d54a-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="0d54a-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d54a-115">Properties</span></span>
| <span data-ttu-id="0d54a-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d54a-116">Property</span></span>     | <span data-ttu-id="0d54a-117">型</span><span class="sxs-lookup"><span data-stu-id="0d54a-117">Type</span></span>   |<span data-ttu-id="0d54a-118">説明</span><span class="sxs-lookup"><span data-stu-id="0d54a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d54a-119">id</span><span class="sxs-lookup"><span data-stu-id="0d54a-119">id</span></span>|<span data-ttu-id="0d54a-120">String</span><span class="sxs-lookup"><span data-stu-id="0d54a-120">String</span></span>|<span data-ttu-id="0d54a-121">カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0d54a-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="0d54a-122">displayName</span><span class="sxs-lookup"><span data-stu-id="0d54a-122">displayName</span></span>|<span data-ttu-id="0d54a-123">String</span><span class="sxs-lookup"><span data-stu-id="0d54a-123">String</span></span>|<span data-ttu-id="0d54a-124">カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0d54a-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d54a-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d54a-125">JSON representation</span></span>

<span data-ttu-id="0d54a-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0d54a-126">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcategory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
