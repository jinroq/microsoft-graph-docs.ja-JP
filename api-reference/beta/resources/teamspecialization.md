---
title: teamspecialization 列挙型
description: チームの特別なユースケースについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553653"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="df1da-103">teamspecialization 列挙型</span><span class="sxs-lookup"><span data-stu-id="df1da-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df1da-104">[チーム](../resources/team.md)が特定のユースケースを対象としているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="df1da-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="df1da-105">各[チーム](../resources/team.md)の特殊化は、そのユースケースを対象とした固有の動作とエクスペリエンスにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="df1da-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="df1da-106">既定値は ' none ' です。</span><span class="sxs-lookup"><span data-stu-id="df1da-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="df1da-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="df1da-107">Members</span></span>

| <span data-ttu-id="df1da-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="df1da-108">Member</span></span>             | <span data-ttu-id="df1da-109">値</span><span class="sxs-lookup"><span data-stu-id="df1da-109">Value</span></span> | <span data-ttu-id="df1da-110">説明</span><span class="sxs-lookup"><span data-stu-id="df1da-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="df1da-111">なし</span><span class="sxs-lookup"><span data-stu-id="df1da-111">none</span></span>               | <span data-ttu-id="df1da-112">.0</span><span class="sxs-lookup"><span data-stu-id="df1da-112">0</span></span>     | <span data-ttu-id="df1da-113">標準のチーム環境を提供するチームの既定の種類。</span><span class="sxs-lookup"><span data-stu-id="df1da-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="df1da-114">educationStandard</span><span class="sxs-lookup"><span data-stu-id="df1da-114">educationStandard</span></span>  | <span data-ttu-id="df1da-115">1 </span><span class="sxs-lookup"><span data-stu-id="df1da-115">1</span></span>     | <span data-ttu-id="df1da-116">教育機関ユーザーによって作成されたチーム。</span><span class="sxs-lookup"><span data-stu-id="df1da-116">Team created by an education user.</span></span> <span data-ttu-id="df1da-117">教育機関のユーザーによって作成されたすべてのチームの種類は Edu です。</span><span class="sxs-lookup"><span data-stu-id="df1da-117">All teams created by education user are of type Edu.</span></span> |
| <span data-ttu-id="df1da-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="df1da-118">educationClass</span></span>     | <span data-ttu-id="df1da-119">2 </span><span class="sxs-lookup"><span data-stu-id="df1da-119">2</span></span>     | <span data-ttu-id="df1da-120">クラスに対して最適化されたチームの作業環境。</span><span class="sxs-lookup"><span data-stu-id="df1da-120">Team experience optimized for a class.</span></span> <span data-ttu-id="df1da-121">これにより、O365 間での機能のセグメンテーションが可能になります。</span><span class="sxs-lookup"><span data-stu-id="df1da-121">This enables segmentation of features across O365.</span></span> |
| <span data-ttu-id="df1da-122">educationProfessionalLearningCommunity</span><span class="sxs-lookup"><span data-stu-id="df1da-122">educationProfessionalLearningCommunity</span></span> | <span data-ttu-id="df1da-123">3 </span><span class="sxs-lookup"><span data-stu-id="df1da-123">3</span></span> | <span data-ttu-id="df1da-124">PLC 用に最適化されたチームの作業環境。</span><span class="sxs-lookup"><span data-stu-id="df1da-124">Team experience optimized for a PLC.</span></span> <span data-ttu-id="df1da-125">[この記事](https://en.wikipedia.org/wiki/Professional_learning_community)の「PLC」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df1da-125">Learn more about PLC [here](https://en.wikipedia.org/wiki/Professional_learning_community).</span></span> |
| <span data-ttu-id="df1da-126">educationStaff</span><span class="sxs-lookup"><span data-stu-id="df1da-126">educationStaff</span></span>     | <span data-ttu-id="df1da-127">4 </span><span class="sxs-lookup"><span data-stu-id="df1da-127">4</span></span>     |  <span data-ttu-id="df1da-128">チームの種類は、組織内のスタッフ (プリンシパルなど) が管理者であり、教師が管理者であり、専門のノートブックを備えたチームのメンバーである場合に最適な環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="df1da-128">Team type for an optimized experience for staff in an organization, where a staff leader, like a principal, is the admin and teachers are members in a team that comes with a specialized notebook.</span></span> <span data-ttu-id="df1da-129">詳細については、「[教育機関向け OneNote スタッフノートブック](https://www.onenote.com/staffnotebookedu)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df1da-129">For more details, see [OneNote staff notebook for education](https://www.onenote.com/staffnotebookedu).</span></span> |
| <span data-ttu-id="df1da-130">unknownfuturevalue という</span><span class="sxs-lookup"><span data-stu-id="df1da-130">unknownFutureValue</span></span> | <span data-ttu-id="df1da-131">7 </span><span class="sxs-lookup"><span data-stu-id="df1da-131">7</span></span>     | <span data-ttu-id="df1da-132">列挙型を今後拡張するためのプレースホルダーとして予約されている Sentinel 値。</span><span class="sxs-lookup"><span data-stu-id="df1da-132">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
