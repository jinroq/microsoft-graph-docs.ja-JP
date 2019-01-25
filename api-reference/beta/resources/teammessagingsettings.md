---
title: teamMessagingSettings リソースの種類
description: メッセージングを構成する設定は、チーム内の参照。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510100"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="25629-103">teamMessagingSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25629-103">teamMessagingSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25629-104">メッセージングを構成する設定は、[チーム](team.md)内の参照。</span><span class="sxs-lookup"><span data-stu-id="25629-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="25629-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25629-105">Properties</span></span>
| <span data-ttu-id="25629-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25629-106">Property</span></span>     | <span data-ttu-id="25629-107">型</span><span class="sxs-lookup"><span data-stu-id="25629-107">Type</span></span>   |<span data-ttu-id="25629-108">説明</span><span class="sxs-lookup"><span data-stu-id="25629-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25629-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="25629-109">allowUserEditMessages</span></span>|<span data-ttu-id="25629-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="25629-110">Boolean</span></span>|<span data-ttu-id="25629-111">場合 true の場合、ユーザーに設定するには、自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="25629-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="25629-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="25629-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="25629-113">ブール値</span><span class="sxs-lookup"><span data-stu-id="25629-113">Boolean</span></span>|<span data-ttu-id="25629-114">場合は true の場合、ユーザーに設定するには、そのメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="25629-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="25629-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="25629-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="25629-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="25629-116">Boolean</span></span>|<span data-ttu-id="25629-117">場合は true の場合、所有者に設定するには、任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="25629-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="25629-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="25629-118">allowTeamMentions</span></span>|<span data-ttu-id="25629-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="25629-119">Boolean</span></span>|<span data-ttu-id="25629-120">場合、参照投稿を許可する @team を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="25629-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="25629-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="25629-121">allowChannelMentions</span></span>|<span data-ttu-id="25629-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="25629-122">Boolean</span></span>|<span data-ttu-id="25629-123">場合、参照投稿を許可する @channel を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="25629-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25629-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="25629-124">JSON representation</span></span>

<span data-ttu-id="25629-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="25629-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teammessagingsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
