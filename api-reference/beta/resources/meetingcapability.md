---
title: meetingCapability リソースの種類
description: 会議の機能が含まれています
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342d264c1f4c670d159c15558c78cc896d4a9487
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931364"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="d6a1b-103">meetingCapability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6a1b-103">meetingCapability resource type</span></span>

> <span data-ttu-id="d6a1b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6a1b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6a1b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6a1b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d6a1b-106">会議の機能が含まれています</span><span class="sxs-lookup"><span data-stu-id="d6a1b-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="d6a1b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6a1b-107">Properties</span></span>

| <span data-ttu-id="d6a1b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6a1b-108">Property</span></span>                          | <span data-ttu-id="d6a1b-109">種類</span><span class="sxs-lookup"><span data-stu-id="d6a1b-109">Type</span></span>    | <span data-ttu-id="d6a1b-110">説明</span><span class="sxs-lookup"><span data-stu-id="d6a1b-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="d6a1b-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="d6a1b-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="d6a1b-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="d6a1b-112">Boolean</span></span> | <span data-ttu-id="d6a1b-113">ダイヤルアウトの匿名ユーザーが会議に出席できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d6a1b-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="d6a1b-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="d6a1b-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="d6a1b-115">ブール型</span><span class="sxs-lookup"><span data-stu-id="d6a1b-115">Boolean</span></span> | <span data-ttu-id="d6a1b-116">匿名ユーザーが会議を開始できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d6a1b-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="d6a1b-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="d6a1b-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="d6a1b-118">String</span><span class="sxs-lookup"><span data-stu-id="d6a1b-118">String</span></span>  | <span data-ttu-id="d6a1b-119">使用可能な値は、`everyoneInCompany`、`everyone` です。</span><span class="sxs-lookup"><span data-stu-id="d6a1b-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="d6a1b-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6a1b-120">JSON representation</span></span>

<span data-ttu-id="d6a1b-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d6a1b-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
