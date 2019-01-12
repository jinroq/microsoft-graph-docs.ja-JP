---
title: teamMessagingSettings リソースの種類
description: メッセージングを構成する設定は、チーム内の参照。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342062ee9661758c8b3179e21246b9366d832f3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930405"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="d3806-103">teamMessagingSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3806-103">teamMessagingSettings resource type</span></span>

> <span data-ttu-id="d3806-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d3806-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3806-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3806-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3806-106">メッセージングを構成する設定は、[チーム](team.md)内の参照。</span><span class="sxs-lookup"><span data-stu-id="d3806-106">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d3806-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3806-107">Properties</span></span>
| <span data-ttu-id="d3806-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3806-108">Property</span></span>     | <span data-ttu-id="d3806-109">種類</span><span class="sxs-lookup"><span data-stu-id="d3806-109">Type</span></span>   |<span data-ttu-id="d3806-110">説明</span><span class="sxs-lookup"><span data-stu-id="d3806-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3806-111">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="d3806-111">allowUserEditMessages</span></span>|<span data-ttu-id="d3806-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="d3806-112">Boolean</span></span>|<span data-ttu-id="d3806-113">場合 true の場合、ユーザーに設定するには、自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="d3806-113">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="d3806-114">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="d3806-114">allowUserDeleteMessages</span></span>|<span data-ttu-id="d3806-115">ブール型</span><span class="sxs-lookup"><span data-stu-id="d3806-115">Boolean</span></span>|<span data-ttu-id="d3806-116">場合は true の場合、ユーザーに設定するには、そのメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="d3806-116">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="d3806-117">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="d3806-117">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="d3806-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="d3806-118">Boolean</span></span>|<span data-ttu-id="d3806-119">場合は true の場合、所有者に設定するには、任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="d3806-119">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="d3806-120">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="d3806-120">allowTeamMentions</span></span>|<span data-ttu-id="d3806-121">ブール型</span><span class="sxs-lookup"><span data-stu-id="d3806-121">Boolean</span></span>|<span data-ttu-id="d3806-122">場合、参照投稿を許可する @team を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="d3806-122">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="d3806-123">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="d3806-123">allowChannelMentions</span></span>|<span data-ttu-id="d3806-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="d3806-124">Boolean</span></span>|<span data-ttu-id="d3806-125">場合、参照投稿を許可する @channel を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="d3806-125">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3806-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3806-126">JSON representation</span></span>

<span data-ttu-id="d3806-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3806-127">The following is a JSON representation of the resource.</span></span>

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
