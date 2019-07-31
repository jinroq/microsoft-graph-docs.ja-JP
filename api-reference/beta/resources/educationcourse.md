---
title: educationCourse リソースの種類
description: クラスのコース情報を表します。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c160f9bd20f7dfccfa19dbf4d466dd967fde9c2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972762"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="eb0aa-103">educationCourse リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eb0aa-103">educationCourse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb0aa-104">クラスのコース情報を表します。</span><span class="sxs-lookup"><span data-stu-id="eb0aa-104">Represents the course information for a class.</span></span> <span data-ttu-id="eb0aa-105">[educationClass](educationclass.md) 内で使用します。</span><span class="sxs-lookup"><span data-stu-id="eb0aa-105">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="eb0aa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb0aa-106">Properties</span></span>

| <span data-ttu-id="eb0aa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb0aa-107">Property</span></span>     | <span data-ttu-id="eb0aa-108">型</span><span class="sxs-lookup"><span data-stu-id="eb0aa-108">Type</span></span>   | <span data-ttu-id="eb0aa-109">説明</span><span class="sxs-lookup"><span data-stu-id="eb0aa-109">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="eb0aa-110">courseNumber</span><span class="sxs-lookup"><span data-stu-id="eb0aa-110">courseNumber</span></span> | <span data-ttu-id="eb0aa-111">String</span><span class="sxs-lookup"><span data-stu-id="eb0aa-111">String</span></span> | <span data-ttu-id="eb0aa-112">コースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="eb0aa-112">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="eb0aa-113">description</span><span class="sxs-lookup"><span data-stu-id="eb0aa-113">description</span></span>  | <span data-ttu-id="eb0aa-114">String</span><span class="sxs-lookup"><span data-stu-id="eb0aa-114">String</span></span> | <span data-ttu-id="eb0aa-115">コースの説明。</span><span class="sxs-lookup"><span data-stu-id="eb0aa-115">Description of the course.</span></span>                |
| <span data-ttu-id="eb0aa-116">displayName</span><span class="sxs-lookup"><span data-stu-id="eb0aa-116">displayName</span></span>  | <span data-ttu-id="eb0aa-117">文字列</span><span class="sxs-lookup"><span data-stu-id="eb0aa-117">String</span></span> | <span data-ttu-id="eb0aa-118">コースの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="eb0aa-118">Name of the course.</span></span>                       |
| <span data-ttu-id="eb0aa-119">externalId</span><span class="sxs-lookup"><span data-stu-id="eb0aa-119">externalId</span></span>   | <span data-ttu-id="eb0aa-120">String</span><span class="sxs-lookup"><span data-stu-id="eb0aa-120">String</span></span> | <span data-ttu-id="eb0aa-121">同期システムからのコースの ID。</span><span class="sxs-lookup"><span data-stu-id="eb0aa-121">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="eb0aa-122">subject</span><span class="sxs-lookup"><span data-stu-id="eb0aa-122">subject</span></span>      | <span data-ttu-id="eb0aa-123">String</span><span class="sxs-lookup"><span data-stu-id="eb0aa-123">String</span></span> | <span data-ttu-id="eb0aa-124">コースの件名。</span><span class="sxs-lookup"><span data-stu-id="eb0aa-124">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="eb0aa-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb0aa-125">JSON representation</span></span>

<span data-ttu-id="eb0aa-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eb0aa-126">The following is a JSON representation of the resource.</span></span>

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
