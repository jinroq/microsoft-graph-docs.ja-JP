---
title: メンバー
description: 'チームの可視性を説明します。 '
ms.openlocfilehash: ecda300ae3a7ce71294e370ce04e9bdc288d8b57
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209727"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="23bd8-103">teamVisibilityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="23bd8-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="23bd8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23bd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23bd8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23bd8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23bd8-106">[チーム](../resources/team.md)の可視性を説明します。</span><span class="sxs-lookup"><span data-stu-id="23bd8-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="23bd8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="23bd8-107">Members</span></span>

| <span data-ttu-id="23bd8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="23bd8-108">Member</span></span> | <span data-ttu-id="23bd8-109">値</span><span class="sxs-lookup"><span data-stu-id="23bd8-109">Value</span></span>| <span data-ttu-id="23bd8-110">説明</span><span class="sxs-lookup"><span data-stu-id="23bd8-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="23bd8-111">プライベート</span><span class="sxs-lookup"><span data-stu-id="23bd8-111">private</span></span>|<span data-ttu-id="23bd8-112">0</span><span class="sxs-lookup"><span data-stu-id="23bd8-112">0</span></span>|<span data-ttu-id="23bd8-113">すべてのユーザー、チームを参照してくださいが、所有者のみがチームにユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="23bd8-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="23bd8-114">public</span><span class="sxs-lookup"><span data-stu-id="23bd8-114">public</span></span>|<span data-ttu-id="23bd8-115">1</span><span class="sxs-lookup"><span data-stu-id="23bd8-115">1</span></span>|<span data-ttu-id="23bd8-116">チームでだれでも参加できます。</span><span class="sxs-lookup"><span data-stu-id="23bd8-116">Anyone can join the team.</span></span>|
