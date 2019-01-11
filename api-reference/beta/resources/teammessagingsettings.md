---
title: teamMessagingSettings リソースの種類
description: メッセージングを構成する設定は、チーム内の参照。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06aca84355a07052dcea316145dfff437eee743b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848259"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="b7e72-103">teamMessagingSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7e72-103">teamMessagingSettings resource type</span></span>

> <span data-ttu-id="b7e72-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7e72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7e72-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7e72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7e72-106">メッセージングを構成する設定は、[チーム](team.md)内の参照。</span><span class="sxs-lookup"><span data-stu-id="b7e72-106">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b7e72-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7e72-107">Properties</span></span>
| <span data-ttu-id="b7e72-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7e72-108">Property</span></span>     | <span data-ttu-id="b7e72-109">種類</span><span class="sxs-lookup"><span data-stu-id="b7e72-109">Type</span></span>   |<span data-ttu-id="b7e72-110">説明</span><span class="sxs-lookup"><span data-stu-id="b7e72-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7e72-111">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="b7e72-111">allowUserEditMessages</span></span>|<span data-ttu-id="b7e72-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7e72-112">Boolean</span></span>|<span data-ttu-id="b7e72-113">場合 true の場合、ユーザーに設定するには、自分のメッセージを編集できます。</span><span class="sxs-lookup"><span data-stu-id="b7e72-113">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="b7e72-114">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="b7e72-114">allowUserDeleteMessages</span></span>|<span data-ttu-id="b7e72-115">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7e72-115">Boolean</span></span>|<span data-ttu-id="b7e72-116">場合は true の場合、ユーザーに設定するには、そのメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="b7e72-116">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="b7e72-117">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="b7e72-117">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="b7e72-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7e72-118">Boolean</span></span>|<span data-ttu-id="b7e72-119">場合は true の場合、所有者に設定するには、任意のメッセージを削除できます。</span><span class="sxs-lookup"><span data-stu-id="b7e72-119">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="b7e72-120">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="b7e72-120">allowTeamMentions</span></span>|<span data-ttu-id="b7e72-121">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7e72-121">Boolean</span></span>|<span data-ttu-id="b7e72-122">場合、参照投稿を許可する @team を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="b7e72-122">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="b7e72-123">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="b7e72-123">allowChannelMentions</span></span>|<span data-ttu-id="b7e72-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="b7e72-124">Boolean</span></span>|<span data-ttu-id="b7e72-125">場合、参照投稿を許可する @channel を true に設定します。</span><span class="sxs-lookup"><span data-stu-id="b7e72-125">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7e72-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7e72-126">JSON representation</span></span>

<span data-ttu-id="b7e72-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7e72-127">The following is a JSON representation of the resource.</span></span>

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
