---
title: Members
description: 'チームの可視性を説明します。 '
author: nkramer
ms.openlocfilehash: 5f03eb52a5eb7aa672998897e11fb5d3a358bf9a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305293"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="ccd5c-103">teamVisibilityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ccd5c-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="ccd5c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ccd5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccd5c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccd5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ccd5c-106">[チーム](../resources/team.md)の可視性を説明します。</span><span class="sxs-lookup"><span data-stu-id="ccd5c-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="ccd5c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ccd5c-107">Members</span></span>

| <span data-ttu-id="ccd5c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ccd5c-108">Member</span></span> | <span data-ttu-id="ccd5c-109">値</span><span class="sxs-lookup"><span data-stu-id="ccd5c-109">Value</span></span>| <span data-ttu-id="ccd5c-110">説明</span><span class="sxs-lookup"><span data-stu-id="ccd5c-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ccd5c-111">プライベート</span><span class="sxs-lookup"><span data-stu-id="ccd5c-111">private</span></span>|<span data-ttu-id="ccd5c-112">0</span><span class="sxs-lookup"><span data-stu-id="ccd5c-112">0</span></span>|<span data-ttu-id="ccd5c-113">すべてのユーザー、チームを参照してくださいが、所有者のみがチームにユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="ccd5c-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="ccd5c-114">public</span><span class="sxs-lookup"><span data-stu-id="ccd5c-114">public</span></span>|<span data-ttu-id="ccd5c-115">1</span><span class="sxs-lookup"><span data-stu-id="ccd5c-115">1</span></span>|<span data-ttu-id="ccd5c-116">チームでだれでも参加できます。</span><span class="sxs-lookup"><span data-stu-id="ccd5c-116">Anyone can join the team.</span></span>|
