---
title: meetingCapability リソースの種類
description: 会議の機能が含まれています
ms.openlocfilehash: 438193d08ab5542f07d4cbf61704520d81433e50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069750"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="6c5de-103">meetingCapability リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c5de-103">meetingCapability resource type</span></span>

> <span data-ttu-id="6c5de-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c5de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c5de-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c5de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c5de-106">会議の機能が含まれています</span><span class="sxs-lookup"><span data-stu-id="6c5de-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="6c5de-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c5de-107">Properties</span></span>

| <span data-ttu-id="6c5de-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c5de-108">Property</span></span>       | <span data-ttu-id="6c5de-109">型</span><span class="sxs-lookup"><span data-stu-id="6c5de-109">Type</span></span>    | <span data-ttu-id="6c5de-110">説明</span><span class="sxs-lookup"><span data-stu-id="6c5de-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6c5de-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="6c5de-111">allowAnonymousUsersToDialOut</span></span> | <span data-ttu-id="6c5de-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="6c5de-112">Boolean</span></span> | <span data-ttu-id="6c5de-113">ダイヤルアウトの匿名ユーザーが会議に出席できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6c5de-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="6c5de-114">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="6c5de-114">autoAdmittedUsers</span></span> | <span data-ttu-id="6c5de-115">String</span><span class="sxs-lookup"><span data-stu-id="6c5de-115">String</span></span> | <span data-ttu-id="6c5de-116">使用可能な値は、`everyoneInCompany`、`everyone` です。</span><span class="sxs-lookup"><span data-stu-id="6c5de-116">Possible values are: `everyoneInCompany`, `everyone`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6c5de-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c5de-117">JSON representation</span></span>

<span data-ttu-id="6c5de-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6c5de-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
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
