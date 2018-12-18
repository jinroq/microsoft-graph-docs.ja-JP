---
title: educationTeacher リソースの種類
description: ユーザーの primaryRole が `teacher` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
ms.openlocfilehash: ca174381fe8722c5b96848ced1d0e09b469068f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351661"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="6e651-103">educationTeacher リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e651-103">educationTeacher resource type</span></span>

> <span data-ttu-id="6e651-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6e651-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e651-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e651-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e651-106">ユーザーの primaryRole が `teacher` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="6e651-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="6e651-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e651-107">Properties</span></span>
| <span data-ttu-id="6e651-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e651-108">Property</span></span>     | <span data-ttu-id="6e651-109">種類</span><span class="sxs-lookup"><span data-stu-id="6e651-109">Type</span></span>   |<span data-ttu-id="6e651-110">説明</span><span class="sxs-lookup"><span data-stu-id="6e651-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e651-111">externalId</span><span class="sxs-lookup"><span data-stu-id="6e651-111">externalId</span></span>|<span data-ttu-id="6e651-112">String</span><span class="sxs-lookup"><span data-stu-id="6e651-112">String</span></span>| <span data-ttu-id="6e651-113">ソース システムの教師の ID。</span><span class="sxs-lookup"><span data-stu-id="6e651-113">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="6e651-114">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="6e651-114">teacherNumber</span></span>|<span data-ttu-id="6e651-115">String</span><span class="sxs-lookup"><span data-stu-id="6e651-115">String</span></span>|<span data-ttu-id="6e651-116">教師の番号。</span><span class="sxs-lookup"><span data-stu-id="6e651-116">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e651-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e651-117">JSON representation</span></span>

<span data-ttu-id="6e651-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6e651-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->