---
title: teamSpecialization 列挙型
description: チームの特別なユースケースについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: a0ff737b196cc486aa01d5e0f5a34c30edc7c8bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964428"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="58360-103">teamSpecialization 列挙型</span><span class="sxs-lookup"><span data-stu-id="58360-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58360-104">[チーム](../resources/team.md)が特定のユースケースを対象としているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="58360-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="58360-105">各[チーム](../resources/team.md)の特殊化は、そのユースケースを対象とした固有の動作とエクスペリエンスにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="58360-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="58360-106">既定値は ' none ' です。</span><span class="sxs-lookup"><span data-stu-id="58360-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="58360-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="58360-107">Members</span></span>

| <span data-ttu-id="58360-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="58360-108">Member</span></span>             | <span data-ttu-id="58360-109">値</span><span class="sxs-lookup"><span data-stu-id="58360-109">Value</span></span> | <span data-ttu-id="58360-110">説明</span><span class="sxs-lookup"><span data-stu-id="58360-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="58360-111">none</span><span class="sxs-lookup"><span data-stu-id="58360-111">none</span></span>               | <span data-ttu-id="58360-112">.0</span><span class="sxs-lookup"><span data-stu-id="58360-112">0</span></span>     | <span data-ttu-id="58360-113">標準のチーム環境を提供するチームの既定の種類。</span><span class="sxs-lookup"><span data-stu-id="58360-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="58360-114">educationStandard</span><span class="sxs-lookup"><span data-stu-id="58360-114">educationStandard</span></span>  | <span data-ttu-id="58360-115">1-d</span><span class="sxs-lookup"><span data-stu-id="58360-115">1</span></span>     | <span data-ttu-id="58360-116">教育機関ユーザーによって作成されたチーム。</span><span class="sxs-lookup"><span data-stu-id="58360-116">Team created by an education user.</span></span> <span data-ttu-id="58360-117">教育機関のユーザーによって作成されたすべてのチームの種類は Edu です。</span><span class="sxs-lookup"><span data-stu-id="58360-117">All teams created by education user are of type Edu.</span></span> |
| <span data-ttu-id="58360-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="58360-118">educationClass</span></span>     | <span data-ttu-id="58360-119">pbm-2</span><span class="sxs-lookup"><span data-stu-id="58360-119">2</span></span>     | <span data-ttu-id="58360-120">クラスに対して最適化されたチームの作業環境。</span><span class="sxs-lookup"><span data-stu-id="58360-120">Team experience optimized for a class.</span></span> <span data-ttu-id="58360-121">これにより、O365 間での機能のセグメンテーションが可能になります。</span><span class="sxs-lookup"><span data-stu-id="58360-121">This enables segmentation of features across O365.</span></span> |
| <span data-ttu-id="58360-122">educationProfessionalLearningCommunity</span><span class="sxs-lookup"><span data-stu-id="58360-122">educationProfessionalLearningCommunity</span></span> | <span data-ttu-id="58360-123">1/3</span><span class="sxs-lookup"><span data-stu-id="58360-123">3</span></span> | <span data-ttu-id="58360-124">PLC 用に最適化されたチームの作業環境。</span><span class="sxs-lookup"><span data-stu-id="58360-124">Team experience optimized for a PLC.</span></span> <span data-ttu-id="58360-125">[この記事](https://en.wikipedia.org/wiki/Professional_learning_community)の「PLC」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58360-125">Learn more about PLC [here](https://en.wikipedia.org/wiki/Professional_learning_community).</span></span> |
| <span data-ttu-id="58360-126">educationStaff</span><span class="sxs-lookup"><span data-stu-id="58360-126">educationStaff</span></span>     | <span data-ttu-id="58360-127">2/4</span><span class="sxs-lookup"><span data-stu-id="58360-127">4</span></span>     |  <span data-ttu-id="58360-128">チームの種類は、組織内のスタッフ (プリンシパルなど) が管理者であり、教師が管理者であり、専門のノートブックを備えたチームのメンバーである場合に最適な環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="58360-128">Team type for an optimized experience for staff in an organization, where a staff leader, like a principal, is the admin and teachers are members in a team that comes with a specialized notebook.</span></span> <span data-ttu-id="58360-129">詳細については、「[教育機関向け OneNote スタッフノートブック](https://www.onenote.com/staffnotebookedu)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58360-129">For more details, see [OneNote staff notebook for education](https://www.onenote.com/staffnotebookedu).</span></span> |
| <span data-ttu-id="58360-130">Unknownfuturevalue という</span><span class="sxs-lookup"><span data-stu-id="58360-130">unknownFutureValue</span></span> | <span data-ttu-id="58360-131">7</span><span class="sxs-lookup"><span data-stu-id="58360-131">7</span></span>     | <span data-ttu-id="58360-132">列挙型を今後拡張するためのプレースホルダーとして予約されている Sentinel 値。</span><span class="sxs-lookup"><span data-stu-id="58360-132">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
