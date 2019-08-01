---
title: teamMessagingSettings リソースの種類
description: チームでメッセージとメンションを構成する設定。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 27ef5062e84f20dc1dbf6be11020f421871fbc09
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033839"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="5ca9a-103">teamMessagingSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ca9a-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="5ca9a-104">[チーム](team.md)内のメッセージとメンションを構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="5ca9a-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5ca9a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ca9a-105">Properties</span></span>
| <span data-ttu-id="5ca9a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ca9a-106">Property</span></span>     | <span data-ttu-id="5ca9a-107">型</span><span class="sxs-lookup"><span data-stu-id="5ca9a-107">Type</span></span>   |<span data-ttu-id="5ca9a-108">説明</span><span class="sxs-lookup"><span data-stu-id="5ca9a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ca9a-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="5ca9a-109">allowUserEditMessages</span></span>|<span data-ttu-id="5ca9a-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ca9a-110">Boolean</span></span>|<span data-ttu-id="5ca9a-111">True に設定されている場合、ユーザーは自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="5ca9a-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="5ca9a-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="5ca9a-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="5ca9a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ca9a-113">Boolean</span></span>|<span data-ttu-id="5ca9a-114">True に設定されている場合、ユーザーは自分のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="5ca9a-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="5ca9a-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="5ca9a-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="5ca9a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ca9a-116">Boolean</span></span>|<span data-ttu-id="5ca9a-117">True に設定されている場合、所有者は任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="5ca9a-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="5ca9a-118">allowTeamMentions ション</span><span class="sxs-lookup"><span data-stu-id="5ca9a-118">allowTeamMentions</span></span>|<span data-ttu-id="5ca9a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ca9a-119">Boolean</span></span>|<span data-ttu-id="5ca9a-120">True に設定すると @team メンションが許可されます。</span><span class="sxs-lookup"><span data-stu-id="5ca9a-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="5ca9a-121">allowChannelMentions ション</span><span class="sxs-lookup"><span data-stu-id="5ca9a-121">allowChannelMentions</span></span>|<span data-ttu-id="5ca9a-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ca9a-122">Boolean</span></span>|<span data-ttu-id="5ca9a-123">True に設定すると @channel メンションが許可されます。</span><span class="sxs-lookup"><span data-stu-id="5ca9a-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ca9a-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ca9a-124">JSON representation</span></span>

<span data-ttu-id="5ca9a-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ca9a-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
