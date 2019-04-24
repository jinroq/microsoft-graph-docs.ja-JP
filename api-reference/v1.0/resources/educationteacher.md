---
title: educationTeacher リソースの種類
description: ユーザーの primaryRole が `teacher` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b58d74e6b53b1721a5139d050c7e89197b8721be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463657"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="6b533-103">educationTeacher リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b533-103">educationTeacher resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b533-104">ユーザーの primaryRole が `teacher` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="6b533-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="6b533-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b533-105">Properties</span></span>
| <span data-ttu-id="6b533-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b533-106">Property</span></span>     | <span data-ttu-id="6b533-107">型</span><span class="sxs-lookup"><span data-stu-id="6b533-107">Type</span></span>   |<span data-ttu-id="6b533-108">説明</span><span class="sxs-lookup"><span data-stu-id="6b533-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b533-109">externalId</span><span class="sxs-lookup"><span data-stu-id="6b533-109">externalId</span></span>|<span data-ttu-id="6b533-110">String</span><span class="sxs-lookup"><span data-stu-id="6b533-110">String</span></span>| <span data-ttu-id="6b533-111">ソース システムの教師の ID。</span><span class="sxs-lookup"><span data-stu-id="6b533-111">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="6b533-112">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="6b533-112">teacherNumber</span></span>|<span data-ttu-id="6b533-113">String</span><span class="sxs-lookup"><span data-stu-id="6b533-113">String</span></span>|<span data-ttu-id="6b533-114">教師の番号。</span><span class="sxs-lookup"><span data-stu-id="6b533-114">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b533-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b533-115">JSON representation</span></span>

<span data-ttu-id="6b533-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b533-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationteacher.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
