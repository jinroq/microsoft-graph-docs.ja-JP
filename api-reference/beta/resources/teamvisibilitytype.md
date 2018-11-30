---
title: メンバー
description: 'チームの可視性を説明します。 '
ms.openlocfilehash: 0e2e9773f8134bb48f317aef1b71a1ca77f26aae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073140"
---
#<a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="97b15-103">teamVisibilityType 列挙型</span><span class="sxs-lookup"><span data-stu-id="97b15-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="97b15-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="97b15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97b15-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97b15-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97b15-106">[チーム](../resources/team.md)の可視性を説明します。</span><span class="sxs-lookup"><span data-stu-id="97b15-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="97b15-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="97b15-107">Members</span></span>

| <span data-ttu-id="97b15-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="97b15-108">Member</span></span> | <span data-ttu-id="97b15-109">値</span><span class="sxs-lookup"><span data-stu-id="97b15-109">Value</span></span>| <span data-ttu-id="97b15-110">説明</span><span class="sxs-lookup"><span data-stu-id="97b15-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="97b15-111">プライベート</span><span class="sxs-lookup"><span data-stu-id="97b15-111">private</span></span>|<span data-ttu-id="97b15-112">0</span><span class="sxs-lookup"><span data-stu-id="97b15-112">0</span></span>|<span data-ttu-id="97b15-113">すべてのユーザー、チームを参照してくださいが、所有者のみがチームにユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="97b15-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="97b15-114">public</span><span class="sxs-lookup"><span data-stu-id="97b15-114">public</span></span>|<span data-ttu-id="97b15-115">1</span><span class="sxs-lookup"><span data-stu-id="97b15-115">1</span></span>|<span data-ttu-id="97b15-116">チームでだれでも参加できます。</span><span class="sxs-lookup"><span data-stu-id="97b15-116">Anyone can join the team.</span></span>|
