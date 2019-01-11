---
title: educationTeacher リソースの種類
description: ユーザーの primaryRole が `teacher` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: eece9080c34855d4546321b7605b47f4b2f231a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875965"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="8003b-103">educationTeacher リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8003b-103">educationTeacher resource type</span></span>

> <span data-ttu-id="8003b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8003b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8003b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8003b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8003b-106">ユーザーの primaryRole が `teacher` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="8003b-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="8003b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8003b-107">Properties</span></span>
| <span data-ttu-id="8003b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8003b-108">Property</span></span>     | <span data-ttu-id="8003b-109">種類</span><span class="sxs-lookup"><span data-stu-id="8003b-109">Type</span></span>   |<span data-ttu-id="8003b-110">説明</span><span class="sxs-lookup"><span data-stu-id="8003b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8003b-111">externalId</span><span class="sxs-lookup"><span data-stu-id="8003b-111">externalId</span></span>|<span data-ttu-id="8003b-112">String</span><span class="sxs-lookup"><span data-stu-id="8003b-112">String</span></span>| <span data-ttu-id="8003b-113">ソース システムの教師の ID。</span><span class="sxs-lookup"><span data-stu-id="8003b-113">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="8003b-114">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="8003b-114">teacherNumber</span></span>|<span data-ttu-id="8003b-115">String</span><span class="sxs-lookup"><span data-stu-id="8003b-115">String</span></span>|<span data-ttu-id="8003b-116">教師の番号。</span><span class="sxs-lookup"><span data-stu-id="8003b-116">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8003b-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8003b-117">JSON representation</span></span>

<span data-ttu-id="8003b-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8003b-118">The following is a JSON representation of the resource.</span></span>

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
