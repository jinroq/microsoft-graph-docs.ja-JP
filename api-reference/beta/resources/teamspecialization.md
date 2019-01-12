---
title: teamSpecialization 列挙型
description: チームの特別なユース ケースをについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a2272ee085d0c265adc9ce2e3f1c598e45be21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930286"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="8470a-103">teamSpecialization 列挙型</span><span class="sxs-lookup"><span data-stu-id="8470a-103">teamSpecialization enum type</span></span>

> <span data-ttu-id="8470a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8470a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8470a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8470a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8470a-106">[チーム](../resources/team.md)が特定のユース ケースの目的として かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8470a-106">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="8470a-107">各[チーム](../resources/team.md)の特殊化では、固有の動作とその使用例を対象としての経験へのアクセスを持ちます。</span><span class="sxs-lookup"><span data-stu-id="8470a-107">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="8470a-108">既定では 'なし' です。</span><span class="sxs-lookup"><span data-stu-id="8470a-108">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="8470a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8470a-109">Members</span></span>

| <span data-ttu-id="8470a-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="8470a-110">Member</span></span>             | <span data-ttu-id="8470a-111">値</span><span class="sxs-lookup"><span data-stu-id="8470a-111">Value</span></span> | <span data-ttu-id="8470a-112">説明</span><span class="sxs-lookup"><span data-stu-id="8470a-112">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="8470a-113">none</span><span class="sxs-lookup"><span data-stu-id="8470a-113">none</span></span>               | <span data-ttu-id="8470a-114">0</span><span class="sxs-lookup"><span data-stu-id="8470a-114">0</span></span>     | <span data-ttu-id="8470a-115">既定の標準的なチームの経験を提供するチームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="8470a-115">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="8470a-116">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="8470a-116">unknownFutureValue</span></span> | <span data-ttu-id="8470a-117">7</span><span class="sxs-lookup"><span data-stu-id="8470a-117">7</span></span>     | <span data-ttu-id="8470a-118">列挙型の将来の拡張用のプレース ホルダーとして予約されている値を sentinel します。</span><span class="sxs-lookup"><span data-stu-id="8470a-118">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
