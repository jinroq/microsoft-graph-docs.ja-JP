---
title: educationTeacher リソースの種類
description: ユーザーの primaryRole が `teacher` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2a94eb2c6a1d145c51fef8c35b3b2f9083cf598a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972333"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="0a7d7-103">educationTeacher リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a7d7-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a7d7-104">ユーザーの primaryRole が `teacher` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="0a7d7-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="0a7d7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a7d7-105">Properties</span></span>
| <span data-ttu-id="0a7d7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a7d7-106">Property</span></span>     | <span data-ttu-id="0a7d7-107">型</span><span class="sxs-lookup"><span data-stu-id="0a7d7-107">Type</span></span>   |<span data-ttu-id="0a7d7-108">説明</span><span class="sxs-lookup"><span data-stu-id="0a7d7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a7d7-109">externalId</span><span class="sxs-lookup"><span data-stu-id="0a7d7-109">externalId</span></span>|<span data-ttu-id="0a7d7-110">String</span><span class="sxs-lookup"><span data-stu-id="0a7d7-110">String</span></span>| <span data-ttu-id="0a7d7-111">ソース システムの教師の ID。</span><span class="sxs-lookup"><span data-stu-id="0a7d7-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="0a7d7-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="0a7d7-112">teacherNumber</span></span>|<span data-ttu-id="0a7d7-113">String</span><span class="sxs-lookup"><span data-stu-id="0a7d7-113">String</span></span>|<span data-ttu-id="0a7d7-114">教師の番号。</span><span class="sxs-lookup"><span data-stu-id="0a7d7-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a7d7-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a7d7-115">JSON representation</span></span>

<span data-ttu-id="0a7d7-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a7d7-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
