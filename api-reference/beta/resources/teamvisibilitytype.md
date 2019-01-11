---
title: メンバー
description: 'チームの可視性を説明します。 '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 21f53b1d7631cde46f1bd70afcbb1346f9199d9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884540"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="23184-103">teamVisibilityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="23184-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="23184-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23184-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23184-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23184-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23184-106">[チーム](../resources/team.md)の可視性を説明します。</span><span class="sxs-lookup"><span data-stu-id="23184-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="23184-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="23184-107">Members</span></span>

| <span data-ttu-id="23184-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="23184-108">Member</span></span> | <span data-ttu-id="23184-109">値</span><span class="sxs-lookup"><span data-stu-id="23184-109">Value</span></span>| <span data-ttu-id="23184-110">説明</span><span class="sxs-lookup"><span data-stu-id="23184-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="23184-111">プライベート</span><span class="sxs-lookup"><span data-stu-id="23184-111">private</span></span>|<span data-ttu-id="23184-112">0</span><span class="sxs-lookup"><span data-stu-id="23184-112">0</span></span>|<span data-ttu-id="23184-113">すべてのユーザー、チームを参照してくださいが、所有者のみがチームにユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="23184-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="23184-114">public</span><span class="sxs-lookup"><span data-stu-id="23184-114">public</span></span>|<span data-ttu-id="23184-115">1</span><span class="sxs-lookup"><span data-stu-id="23184-115">1</span></span>|<span data-ttu-id="23184-116">チームでだれでも参加できます。</span><span class="sxs-lookup"><span data-stu-id="23184-116">Anyone can join the team.</span></span>|
