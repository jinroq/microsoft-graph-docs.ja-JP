---
title: teamSpecialization 列挙型
description: チームの特別なユース ケースをについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9e19c6b2242256f0d1b7a23c89aa07787bfc1913
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522652"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="4f44f-103">teamSpecialization 列挙型</span><span class="sxs-lookup"><span data-stu-id="4f44f-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f44f-104">[チーム](../resources/team.md)が特定のユース ケースの目的として かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4f44f-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="4f44f-105">各[チーム](../resources/team.md)の特殊化では、固有の動作とその使用例を対象としての経験へのアクセスを持ちます。</span><span class="sxs-lookup"><span data-stu-id="4f44f-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="4f44f-106">既定では 'なし' です。</span><span class="sxs-lookup"><span data-stu-id="4f44f-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="4f44f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f44f-107">Members</span></span>

| <span data-ttu-id="4f44f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f44f-108">Member</span></span>             | <span data-ttu-id="4f44f-109">値</span><span class="sxs-lookup"><span data-stu-id="4f44f-109">Value</span></span> | <span data-ttu-id="4f44f-110">説明</span><span class="sxs-lookup"><span data-stu-id="4f44f-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="4f44f-111">none</span><span class="sxs-lookup"><span data-stu-id="4f44f-111">none</span></span>               | <span data-ttu-id="4f44f-112">(0)</span><span class="sxs-lookup"><span data-stu-id="4f44f-112">0</span></span>     | <span data-ttu-id="4f44f-113">既定の標準的なチームの経験を提供するチームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="4f44f-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="4f44f-114">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="4f44f-114">unknownFutureValue</span></span> | <span data-ttu-id="4f44f-115">-7</span><span class="sxs-lookup"><span data-stu-id="4f44f-115">7</span></span>     | <span data-ttu-id="4f44f-116">列挙型の将来の拡張用のプレース ホルダーとして予約されている値を sentinel します。</span><span class="sxs-lookup"><span data-stu-id="4f44f-116">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamspecialization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
