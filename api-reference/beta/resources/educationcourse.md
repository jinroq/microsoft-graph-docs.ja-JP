---
title: educationCourse リソースの種類
description: クラスのコース情報を表します。
author: mlafleur
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eac609f787621e30d4707d477296fc53af77dad0
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764769"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="c4dea-103">educationCourse リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4dea-103">educationCourse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4dea-104">クラスのコース情報を表します。</span><span class="sxs-lookup"><span data-stu-id="c4dea-104">Represents the course information for a class.</span></span> <span data-ttu-id="c4dea-105">[educationClass](educationclass.md) 内で使用します。</span><span class="sxs-lookup"><span data-stu-id="c4dea-105">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c4dea-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4dea-106">Properties</span></span>

| <span data-ttu-id="c4dea-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4dea-107">Property</span></span>     | <span data-ttu-id="c4dea-108">型</span><span class="sxs-lookup"><span data-stu-id="c4dea-108">Type</span></span>   | <span data-ttu-id="c4dea-109">説明</span><span class="sxs-lookup"><span data-stu-id="c4dea-109">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="c4dea-110">courseNumber</span><span class="sxs-lookup"><span data-stu-id="c4dea-110">courseNumber</span></span> | <span data-ttu-id="c4dea-111">String</span><span class="sxs-lookup"><span data-stu-id="c4dea-111">String</span></span> | <span data-ttu-id="c4dea-112">コースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c4dea-112">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="c4dea-113">description</span><span class="sxs-lookup"><span data-stu-id="c4dea-113">description</span></span>  | <span data-ttu-id="c4dea-114">String</span><span class="sxs-lookup"><span data-stu-id="c4dea-114">String</span></span> | <span data-ttu-id="c4dea-115">コースの説明。</span><span class="sxs-lookup"><span data-stu-id="c4dea-115">Description of the course.</span></span>                |
| <span data-ttu-id="c4dea-116">displayName</span><span class="sxs-lookup"><span data-stu-id="c4dea-116">displayName</span></span>  | <span data-ttu-id="c4dea-117">文字列</span><span class="sxs-lookup"><span data-stu-id="c4dea-117">String</span></span> | <span data-ttu-id="c4dea-118">コースの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="c4dea-118">Name of the course.</span></span>                       |
| <span data-ttu-id="c4dea-119">externalId</span><span class="sxs-lookup"><span data-stu-id="c4dea-119">externalId</span></span>   | <span data-ttu-id="c4dea-120">String</span><span class="sxs-lookup"><span data-stu-id="c4dea-120">String</span></span> | <span data-ttu-id="c4dea-121">同期システムからのコースの ID。</span><span class="sxs-lookup"><span data-stu-id="c4dea-121">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="c4dea-122">subject</span><span class="sxs-lookup"><span data-stu-id="c4dea-122">subject</span></span>      | <span data-ttu-id="c4dea-123">String</span><span class="sxs-lookup"><span data-stu-id="c4dea-123">String</span></span> | <span data-ttu-id="c4dea-124">コースの件名。</span><span class="sxs-lookup"><span data-stu-id="c4dea-124">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="c4dea-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4dea-125">JSON representation</span></span>

<span data-ttu-id="c4dea-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c4dea-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCourse"
}-->

```json
{
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationCourse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
