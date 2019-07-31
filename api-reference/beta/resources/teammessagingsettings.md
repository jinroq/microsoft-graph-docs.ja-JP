---
title: teamMessagingSettings リソースの種類
description: チームでメッセージとメンションを構成する設定。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3a89ed35c820338cde7b3f22a7345c860b1a4427
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964530"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="ee655-103">teamMessagingSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee655-103">teamMessagingSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee655-104">[チーム](team.md)内のメッセージとメンションを構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="ee655-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee655-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee655-105">Properties</span></span>
| <span data-ttu-id="ee655-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee655-106">Property</span></span>     | <span data-ttu-id="ee655-107">型</span><span class="sxs-lookup"><span data-stu-id="ee655-107">Type</span></span>   |<span data-ttu-id="ee655-108">説明</span><span class="sxs-lookup"><span data-stu-id="ee655-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee655-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="ee655-109">allowUserEditMessages</span></span>|<span data-ttu-id="ee655-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee655-110">Boolean</span></span>|<span data-ttu-id="ee655-111">True に設定されている場合、ユーザーは自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="ee655-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="ee655-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="ee655-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="ee655-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee655-113">Boolean</span></span>|<span data-ttu-id="ee655-114">True に設定されている場合、ユーザーは自分のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="ee655-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="ee655-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="ee655-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="ee655-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee655-116">Boolean</span></span>|<span data-ttu-id="ee655-117">True に設定されている場合、所有者は任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="ee655-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="ee655-118">allowTeamMentions ション</span><span class="sxs-lookup"><span data-stu-id="ee655-118">allowTeamMentions</span></span>|<span data-ttu-id="ee655-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee655-119">Boolean</span></span>|<span data-ttu-id="ee655-120">True に設定すると @team メンションが許可されます。</span><span class="sxs-lookup"><span data-stu-id="ee655-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="ee655-121">allowChannelMentions ション</span><span class="sxs-lookup"><span data-stu-id="ee655-121">allowChannelMentions</span></span>|<span data-ttu-id="ee655-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee655-122">Boolean</span></span>|<span data-ttu-id="ee655-123">True に設定すると @channel メンションが許可されます。</span><span class="sxs-lookup"><span data-stu-id="ee655-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee655-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee655-124">JSON representation</span></span>

<span data-ttu-id="ee655-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ee655-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
