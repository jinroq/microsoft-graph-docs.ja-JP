---
title: teamMessagingSettings リソースの種類
description: メッセージングを構成する設定は、チーム内の参照。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f8b643b752ab130433153e7a238a64d2960d6705
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967960"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="c9999-103">teamMessagingSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9999-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="c9999-104">メッセージングを構成する設定は、[チーム](team.md)内の参照。</span><span class="sxs-lookup"><span data-stu-id="c9999-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c9999-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9999-105">Properties</span></span>
| <span data-ttu-id="c9999-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9999-106">Property</span></span>     | <span data-ttu-id="c9999-107">種類</span><span class="sxs-lookup"><span data-stu-id="c9999-107">Type</span></span>   |<span data-ttu-id="c9999-108">説明</span><span class="sxs-lookup"><span data-stu-id="c9999-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9999-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="c9999-109">allowUserEditMessages</span></span>|<span data-ttu-id="c9999-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="c9999-110">Boolean</span></span>|<span data-ttu-id="c9999-111">場合 true の場合、ユーザーに設定するには、自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="c9999-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="c9999-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="c9999-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="c9999-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="c9999-113">Boolean</span></span>|<span data-ttu-id="c9999-114">場合は true の場合、ユーザーに設定するには、そのメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="c9999-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="c9999-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="c9999-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="c9999-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="c9999-116">Boolean</span></span>|<span data-ttu-id="c9999-117">場合は true の場合、所有者に設定するには、任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="c9999-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="c9999-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="c9999-118">allowTeamMentions</span></span>|<span data-ttu-id="c9999-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="c9999-119">Boolean</span></span>|<span data-ttu-id="c9999-120">場合、参照投稿を許可する @team を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="c9999-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="c9999-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="c9999-121">allowChannelMentions</span></span>|<span data-ttu-id="c9999-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="c9999-122">Boolean</span></span>|<span data-ttu-id="c9999-123">場合、参照投稿を許可する @channel を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="c9999-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9999-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9999-124">JSON representation</span></span>

<span data-ttu-id="c9999-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c9999-125">The following is a JSON representation of the resource.</span></span>

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
