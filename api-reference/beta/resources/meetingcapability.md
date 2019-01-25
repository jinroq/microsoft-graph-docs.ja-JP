---
title: meetingCapability リソースの種類
description: 会議の機能が含まれています
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e71d7c8c6489d5856e5f2441cd93c7fdea033bd4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524290"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="b9c5a-103">meetingCapability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9c5a-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9c5a-104">会議の機能が含まれています</span><span class="sxs-lookup"><span data-stu-id="b9c5a-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="b9c5a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9c5a-105">Properties</span></span>

| <span data-ttu-id="b9c5a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9c5a-106">Property</span></span>                          | <span data-ttu-id="b9c5a-107">型</span><span class="sxs-lookup"><span data-stu-id="b9c5a-107">Type</span></span>    | <span data-ttu-id="b9c5a-108">説明</span><span class="sxs-lookup"><span data-stu-id="b9c5a-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="b9c5a-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="b9c5a-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="b9c5a-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="b9c5a-110">Boolean</span></span> | <span data-ttu-id="b9c5a-111">ダイヤルアウトの匿名ユーザーが会議に出席できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="b9c5a-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="b9c5a-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="b9c5a-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="b9c5a-113">Boolean</span></span> | <span data-ttu-id="b9c5a-114">匿名ユーザーが会議を開始できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="b9c5a-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="b9c5a-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="b9c5a-116">String</span><span class="sxs-lookup"><span data-stu-id="b9c5a-116">String</span></span>  | <span data-ttu-id="b9c5a-117">使用可能な値は、`everyoneInCompany`、`everyone` です。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="b9c5a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9c5a-118">JSON representation</span></span>

<span data-ttu-id="b9c5a-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9c5a-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingcapability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
