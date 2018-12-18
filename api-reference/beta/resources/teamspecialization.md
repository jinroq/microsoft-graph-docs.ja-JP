---
title: teamSpecialization 列挙型
description: チームの特別なユース ケースをについて説明します。
author: nkramer
ms.openlocfilehash: 2e17f03374457ff8ddd9d3941eb56bebbec2dde6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348014"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="864ac-103">teamSpecialization 列挙型</span><span class="sxs-lookup"><span data-stu-id="864ac-103">teamSpecialization enum type</span></span>

> <span data-ttu-id="864ac-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="864ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="864ac-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="864ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="864ac-106">[チーム](../resources/team.md)が特定のユース ケースの目的として かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="864ac-106">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="864ac-107">各[チーム](../resources/team.md)の特殊化では、固有の動作とその使用例を対象としての経験へのアクセスを持ちます。</span><span class="sxs-lookup"><span data-stu-id="864ac-107">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="864ac-108">既定では 'なし' です。</span><span class="sxs-lookup"><span data-stu-id="864ac-108">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="864ac-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="864ac-109">Members</span></span>

| <span data-ttu-id="864ac-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="864ac-110">Member</span></span>             | <span data-ttu-id="864ac-111">値</span><span class="sxs-lookup"><span data-stu-id="864ac-111">Value</span></span> | <span data-ttu-id="864ac-112">説明</span><span class="sxs-lookup"><span data-stu-id="864ac-112">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="864ac-113">none</span><span class="sxs-lookup"><span data-stu-id="864ac-113">none</span></span>               | <span data-ttu-id="864ac-114">0</span><span class="sxs-lookup"><span data-stu-id="864ac-114">0</span></span>     | <span data-ttu-id="864ac-115">既定の標準的なチームの経験を提供するチームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="864ac-115">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="864ac-116">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="864ac-116">unknownFutureValue</span></span> | <span data-ttu-id="864ac-117">7</span><span class="sxs-lookup"><span data-stu-id="864ac-117">7</span></span>     | <span data-ttu-id="864ac-118">列挙型の将来の拡張用のプレース ホルダーとして予約されている値を sentinel します。</span><span class="sxs-lookup"><span data-stu-id="864ac-118">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
