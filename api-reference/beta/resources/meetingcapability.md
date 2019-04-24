---
title: 会議機能リソースの種類
description: 会議の機能が含まれています。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e71d7c8c6489d5856e5f2441cd93c7fdea033bd4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457145"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="6c5ee-103">会議機能リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c5ee-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c5ee-104">会議の機能が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c5ee-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="6c5ee-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c5ee-105">Properties</span></span>

| <span data-ttu-id="6c5ee-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c5ee-106">Property</span></span>                          | <span data-ttu-id="6c5ee-107">型</span><span class="sxs-lookup"><span data-stu-id="6c5ee-107">Type</span></span>    | <span data-ttu-id="6c5ee-108">説明</span><span class="sxs-lookup"><span data-stu-id="6c5ee-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="6c5ee-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="6c5ee-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="6c5ee-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="6c5ee-110">Boolean</span></span> | <span data-ttu-id="6c5ee-111">匿名ユーザーが会議でダイヤルアウトが許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6c5ee-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="6c5ee-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="6c5ee-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="6c5ee-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="6c5ee-113">Boolean</span></span> | <span data-ttu-id="6c5ee-114">匿名ユーザーが会議の開始を許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6c5ee-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="6c5ee-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="6c5ee-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="6c5ee-116">String</span><span class="sxs-lookup"><span data-stu-id="6c5ee-116">String</span></span>  | <span data-ttu-id="6c5ee-117">使用可能な値は、`everyoneInCompany`、`everyone` です。</span><span class="sxs-lookup"><span data-stu-id="6c5ee-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="6c5ee-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c5ee-118">JSON representation</span></span>

<span data-ttu-id="6c5ee-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c5ee-119">The following is a JSON representation of the resource.</span></span>

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
