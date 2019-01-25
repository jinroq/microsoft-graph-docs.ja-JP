---
title: Members
description: 'チームの可視性を説明します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7e77fbd2667f8656a4c2f66046636ff73ac8891d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521349"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="154da-103">teamVisibilityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="154da-103">teamVisibilityType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="154da-104">[チーム](../resources/team.md)の可視性を説明します。</span><span class="sxs-lookup"><span data-stu-id="154da-104">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="154da-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="154da-105">Members</span></span>

| <span data-ttu-id="154da-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="154da-106">Member</span></span> | <span data-ttu-id="154da-107">値</span><span class="sxs-lookup"><span data-stu-id="154da-107">Value</span></span>| <span data-ttu-id="154da-108">説明</span><span class="sxs-lookup"><span data-stu-id="154da-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="154da-109">Private</span><span class="sxs-lookup"><span data-stu-id="154da-109">private</span></span>|<span data-ttu-id="154da-110">(0)</span><span class="sxs-lookup"><span data-stu-id="154da-110">0</span></span>|<span data-ttu-id="154da-111">すべてのユーザー、チームを参照してくださいが、所有者のみがチームにユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="154da-111">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="154da-112">public</span><span class="sxs-lookup"><span data-stu-id="154da-112">public</span></span>|<span data-ttu-id="154da-113">-1</span><span class="sxs-lookup"><span data-stu-id="154da-113">1</span></span>|<span data-ttu-id="154da-114">チームでだれでも参加できます。</span><span class="sxs-lookup"><span data-stu-id="154da-114">Anyone can join the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamvisibilitytype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
