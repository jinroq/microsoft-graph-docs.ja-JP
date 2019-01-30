---
title: teamSpecialization 列挙型
description: チームの特別なユース ケースをについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640323"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="b4904-103">teamSpecialization 列挙型</span><span class="sxs-lookup"><span data-stu-id="b4904-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4904-104">[チーム](../resources/team.md)が特定のユース ケースの目的として かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b4904-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="b4904-105">各[チーム](../resources/team.md)の特殊化では、固有の動作とその使用例を対象としての経験へのアクセスを持ちます。</span><span class="sxs-lookup"><span data-stu-id="b4904-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="b4904-106">既定では 'なし' です。</span><span class="sxs-lookup"><span data-stu-id="b4904-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="b4904-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b4904-107">Members</span></span>

| <span data-ttu-id="b4904-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b4904-108">Member</span></span>             | <span data-ttu-id="b4904-109">値</span><span class="sxs-lookup"><span data-stu-id="b4904-109">Value</span></span> | <span data-ttu-id="b4904-110">説明</span><span class="sxs-lookup"><span data-stu-id="b4904-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="b4904-111">none</span><span class="sxs-lookup"><span data-stu-id="b4904-111">none</span></span>               | <span data-ttu-id="b4904-112">0</span><span class="sxs-lookup"><span data-stu-id="b4904-112">0</span></span>     | <span data-ttu-id="b4904-113">既定の標準的なチームの経験を提供するチームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="b4904-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="b4904-114">educationStandard</span><span class="sxs-lookup"><span data-stu-id="b4904-114">educationStandard</span></span>  | <span data-ttu-id="b4904-115">1</span><span class="sxs-lookup"><span data-stu-id="b4904-115">1</span></span>     | <span data-ttu-id="b4904-116">教育ユーザーによって作成されたチームです。</span><span class="sxs-lookup"><span data-stu-id="b4904-116">Team created by an education user.</span></span> <span data-ttu-id="b4904-117">教育ユーザーによって作成されたすべてのチームは、Edu の種類です。</span><span class="sxs-lookup"><span data-stu-id="b4904-117">All teams created by education user are of type Edu.</span></span> |
| <span data-ttu-id="b4904-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="b4904-118">educationClass</span></span>     | <span data-ttu-id="b4904-119">2</span><span class="sxs-lookup"><span data-stu-id="b4904-119">2</span></span>     | <span data-ttu-id="b4904-120">クラス用に最適化されたチームの経験。</span><span class="sxs-lookup"><span data-stu-id="b4904-120">Team experience optimized for a class.</span></span> <span data-ttu-id="b4904-121">O365 全体の機能の区分の基準が使用できます。</span><span class="sxs-lookup"><span data-stu-id="b4904-121">This enables segmentation of features across O365.</span></span> |
| <span data-ttu-id="b4904-122">educationProfessionalLearningCommunity</span><span class="sxs-lookup"><span data-stu-id="b4904-122">educationProfessionalLearningCommunity</span></span> | <span data-ttu-id="b4904-123">3</span><span class="sxs-lookup"><span data-stu-id="b4904-123">3</span></span> | <span data-ttu-id="b4904-124">チームの経験を PLC 用に最適化されました。</span><span class="sxs-lookup"><span data-stu-id="b4904-124">Team experience optimized for a PLC.</span></span> <span data-ttu-id="b4904-125">PLC の詳細については[ここで](https://en.wikipedia.org/wiki/Professional_learning_community)。</span><span class="sxs-lookup"><span data-stu-id="b4904-125">Learn more about PLC [here](https://en.wikipedia.org/wiki/Professional_learning_community).</span></span> |
| <span data-ttu-id="b4904-126">educationStaff</span><span class="sxs-lookup"><span data-stu-id="b4904-126">educationStaff</span></span>     | <span data-ttu-id="b4904-127">4</span><span class="sxs-lookup"><span data-stu-id="b4904-127">4</span></span>     |  <span data-ttu-id="b4904-128">管理者、教師、プリンシパルと同様に、スタッフのリーダーは、場所、組織内のスタッフの作業を最適化するためのチーム タイプは、専用のノートブックに付属しているチームのメンバーです。</span><span class="sxs-lookup"><span data-stu-id="b4904-128">Team type for an optimized experience for staff in an organization, where a staff leader, like a principal, is the admin and teachers are members in a team that comes with a specialized notebook.</span></span> <span data-ttu-id="b4904-129">詳細については、[教育のスタッフ ノートを OneNote](https://www.onenote.com/staffnotebookedu)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4904-129">For more details, see [OneNote staff notebook for education](https://www.onenote.com/staffnotebookedu).</span></span> |
| <span data-ttu-id="b4904-130">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="b4904-130">unknownFutureValue</span></span> | <span data-ttu-id="b4904-131">7</span><span class="sxs-lookup"><span data-stu-id="b4904-131">7</span></span>     | <span data-ttu-id="b4904-132">列挙型の将来の拡張用のプレース ホルダーとして予約されている値を sentinel します。</span><span class="sxs-lookup"><span data-stu-id="b4904-132">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
