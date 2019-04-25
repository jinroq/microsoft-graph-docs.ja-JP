---
title: Members
description: 'チームの可視性について説明します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7e77fbd2667f8656a4c2f66046636ff73ac8891d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582942"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="c883b-103">teamVisibilityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c883b-103">teamVisibilityType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c883b-104">[チーム](../resources/team.md)の可視性について説明します。</span><span class="sxs-lookup"><span data-stu-id="c883b-104">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="c883b-105">メンバー</span><span class="sxs-lookup"><span data-stu-id="c883b-105">Members</span></span>

| <span data-ttu-id="c883b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="c883b-106">Member</span></span> | <span data-ttu-id="c883b-107">値</span><span class="sxs-lookup"><span data-stu-id="c883b-107">Value</span></span>| <span data-ttu-id="c883b-108">説明</span><span class="sxs-lookup"><span data-stu-id="c883b-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c883b-109">機密性</span><span class="sxs-lookup"><span data-stu-id="c883b-109">private</span></span>|<span data-ttu-id="c883b-110">.0</span><span class="sxs-lookup"><span data-stu-id="c883b-110">0</span></span>|<span data-ttu-id="c883b-111">チームはだれでも見ることができますが、ユーザーをチームに追加できるのは所有者のみです。</span><span class="sxs-lookup"><span data-stu-id="c883b-111">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="c883b-112">public</span><span class="sxs-lookup"><span data-stu-id="c883b-112">public</span></span>|<span data-ttu-id="c883b-113">1 </span><span class="sxs-lookup"><span data-stu-id="c883b-113">1</span></span>|<span data-ttu-id="c883b-114">すべてのユーザーがチームに参加できます。</span><span class="sxs-lookup"><span data-stu-id="c883b-114">Anyone can join the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamvisibilitytype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
