---
title: メンバー
description: 'チームの可視性を説明します。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b469a4db4bf535eaa4a7c6300a393381c92158fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986444"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="aa346-103">teamVisibilityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="aa346-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="aa346-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa346-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa346-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa346-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa346-106">[チーム](../resources/team.md)の可視性を説明します。</span><span class="sxs-lookup"><span data-stu-id="aa346-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="aa346-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="aa346-107">Members</span></span>

| <span data-ttu-id="aa346-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="aa346-108">Member</span></span> | <span data-ttu-id="aa346-109">値</span><span class="sxs-lookup"><span data-stu-id="aa346-109">Value</span></span>| <span data-ttu-id="aa346-110">説明</span><span class="sxs-lookup"><span data-stu-id="aa346-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aa346-111">プライベート</span><span class="sxs-lookup"><span data-stu-id="aa346-111">private</span></span>|<span data-ttu-id="aa346-112">0</span><span class="sxs-lookup"><span data-stu-id="aa346-112">0</span></span>|<span data-ttu-id="aa346-113">すべてのユーザー、チームを参照してくださいが、所有者のみがチームにユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="aa346-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="aa346-114">public</span><span class="sxs-lookup"><span data-stu-id="aa346-114">public</span></span>|<span data-ttu-id="aa346-115">1</span><span class="sxs-lookup"><span data-stu-id="aa346-115">1</span></span>|<span data-ttu-id="aa346-116">チームでだれでも参加できます。</span><span class="sxs-lookup"><span data-stu-id="aa346-116">Anyone can join the team.</span></span>|
