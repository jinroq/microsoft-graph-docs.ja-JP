---
title: teamMessagingSettings リソースの種類
description: メッセージングを構成する設定は、チーム内の参照。
author: nkramer
ms.openlocfilehash: 387c2e3ccedc6f11f17d4868b1b0d3eaf67624fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304551"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="aee78-103">teamMessagingSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aee78-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="aee78-104">メッセージングを構成する設定は、[チーム](team.md)内の参照。</span><span class="sxs-lookup"><span data-stu-id="aee78-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aee78-105">Properties</span><span class="sxs-lookup"><span data-stu-id="aee78-105">Properties</span></span>
| <span data-ttu-id="aee78-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aee78-106">Property</span></span>     | <span data-ttu-id="aee78-107">種類</span><span class="sxs-lookup"><span data-stu-id="aee78-107">Type</span></span>   |<span data-ttu-id="aee78-108">説明</span><span class="sxs-lookup"><span data-stu-id="aee78-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aee78-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="aee78-109">allowUserEditMessages</span></span>|<span data-ttu-id="aee78-110">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee78-110">Boolean</span></span>|<span data-ttu-id="aee78-111">場合 true の場合、ユーザーに設定するには、自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="aee78-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="aee78-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="aee78-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="aee78-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee78-113">Boolean</span></span>|<span data-ttu-id="aee78-114">場合は true の場合、ユーザーに設定するには、そのメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="aee78-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="aee78-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="aee78-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="aee78-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee78-116">Boolean</span></span>|<span data-ttu-id="aee78-117">場合は true の場合、所有者に設定するには、任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="aee78-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="aee78-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="aee78-118">allowTeamMentions</span></span>|<span data-ttu-id="aee78-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee78-119">Boolean</span></span>|<span data-ttu-id="aee78-120">場合、参照投稿を許可する @team を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="aee78-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="aee78-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="aee78-121">allowChannelMentions</span></span>|<span data-ttu-id="aee78-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="aee78-122">Boolean</span></span>|<span data-ttu-id="aee78-123">場合、参照投稿を許可する @channel を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="aee78-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aee78-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aee78-124">JSON representation</span></span>

<span data-ttu-id="aee78-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aee78-125">The following is a JSON representation of the resource.</span></span>

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
