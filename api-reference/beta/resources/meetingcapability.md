---
title: 会議機能リソースの種類
description: 会議の機能が含まれています。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1de406cf0614a4cbb64749cef763a97a3723eb48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966861"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="df50c-103">会議機能リソースの種類</span><span class="sxs-lookup"><span data-stu-id="df50c-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df50c-104">会議の機能が含まれています。</span><span class="sxs-lookup"><span data-stu-id="df50c-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="df50c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df50c-105">Properties</span></span>

| <span data-ttu-id="df50c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df50c-106">Property</span></span>                          | <span data-ttu-id="df50c-107">型</span><span class="sxs-lookup"><span data-stu-id="df50c-107">Type</span></span>    | <span data-ttu-id="df50c-108">説明</span><span class="sxs-lookup"><span data-stu-id="df50c-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="df50c-109">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="df50c-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="df50c-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="df50c-110">Boolean</span></span> | <span data-ttu-id="df50c-111">匿名ユーザーが会議でダイヤルアウトが許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df50c-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="df50c-112">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="df50c-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="df50c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="df50c-113">Boolean</span></span> | <span data-ttu-id="df50c-114">匿名ユーザーが会議の開始を許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df50c-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="df50c-115">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="df50c-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="df50c-116">String</span><span class="sxs-lookup"><span data-stu-id="df50c-116">String</span></span>  | <span data-ttu-id="df50c-117">使用可能な値は、`everyoneInCompany`、`everyone` です。</span><span class="sxs-lookup"><span data-stu-id="df50c-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="df50c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="df50c-118">JSON representation</span></span>

<span data-ttu-id="df50c-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="df50c-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
