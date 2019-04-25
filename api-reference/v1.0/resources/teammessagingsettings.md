---
title: teammessagingsettings リソースの種類
description: チームでメッセージとメンションを構成する設定。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f8b643b752ab130433153e7a238a64d2960d6705
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573845"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="56894-103">teammessagingsettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56894-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="56894-104">[チーム](team.md)内のメッセージとメンションを構成するための設定。</span><span class="sxs-lookup"><span data-stu-id="56894-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="56894-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56894-105">Properties</span></span>
| <span data-ttu-id="56894-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56894-106">Property</span></span>     | <span data-ttu-id="56894-107">型</span><span class="sxs-lookup"><span data-stu-id="56894-107">Type</span></span>   |<span data-ttu-id="56894-108">説明</span><span class="sxs-lookup"><span data-stu-id="56894-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56894-109">allowusereditmessages</span><span class="sxs-lookup"><span data-stu-id="56894-109">allowUserEditMessages</span></span>|<span data-ttu-id="56894-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="56894-110">Boolean</span></span>|<span data-ttu-id="56894-111">true に設定されている場合、ユーザーは自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="56894-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="56894-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="56894-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="56894-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="56894-113">Boolean</span></span>|<span data-ttu-id="56894-114">true に設定されている場合、ユーザーは自分のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="56894-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="56894-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="56894-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="56894-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="56894-116">Boolean</span></span>|<span data-ttu-id="56894-117">true に設定されている場合、所有者は任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="56894-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="56894-118">allowteammentions ション</span><span class="sxs-lookup"><span data-stu-id="56894-118">allowTeamMentions</span></span>|<span data-ttu-id="56894-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="56894-119">Boolean</span></span>|<span data-ttu-id="56894-120">true に設定すると @team メンションが許可されます。</span><span class="sxs-lookup"><span data-stu-id="56894-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="56894-121">allowchannelmentions ション</span><span class="sxs-lookup"><span data-stu-id="56894-121">allowChannelMentions</span></span>|<span data-ttu-id="56894-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="56894-122">Boolean</span></span>|<span data-ttu-id="56894-123">true に設定すると @channel メンションが許可されます。</span><span class="sxs-lookup"><span data-stu-id="56894-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56894-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56894-124">JSON representation</span></span>

<span data-ttu-id="56894-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="56894-125">The following is a JSON representation of the resource.</span></span>

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
