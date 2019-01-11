---
title: clonableTeamParts 列挙型
description: 'チームのどの部分のクローンを作成する必要があるについて説明します。 '
localization_priority: Normal
ms.openlocfilehash: 7eb71de266ea4f0ed9f94900dd03a47da1a24cc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860558"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="280af-103">clonableTeamParts 列挙型</span><span class="sxs-lookup"><span data-stu-id="280af-103">clonableTeamParts enum type</span></span>

> <span data-ttu-id="280af-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="280af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="280af-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="280af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="280af-106">[チーム](../resources/team.md)のどの部分のクローンを作成する必要があるについて説明します。</span><span class="sxs-lookup"><span data-stu-id="280af-106">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="280af-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="280af-107">Members</span></span>

| <span data-ttu-id="280af-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="280af-108">Member</span></span> | <span data-ttu-id="280af-109">値</span><span class="sxs-lookup"><span data-stu-id="280af-109">Value</span></span>| <span data-ttu-id="280af-110">説明</span><span class="sxs-lookup"><span data-stu-id="280af-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="280af-111">apps</span><span class="sxs-lookup"><span data-stu-id="280af-111">apps</span></span>|<span data-ttu-id="280af-112">1</span><span class="sxs-lookup"><span data-stu-id="280af-112">1</span></span>|<span data-ttu-id="280af-113">インストールされたアプリの一覧をコピーします。</span><span class="sxs-lookup"><span data-stu-id="280af-113">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="280af-114">タブ</span><span class="sxs-lookup"><span data-stu-id="280af-114">tabs</span></span>|<span data-ttu-id="280af-115">2</span><span class="sxs-lookup"><span data-stu-id="280af-115">2</span></span>|<span data-ttu-id="280af-116">チャネル内のタブにコピーします。</span><span class="sxs-lookup"><span data-stu-id="280af-116">copies the tabs within channels.</span></span>|
|<span data-ttu-id="280af-117">settings</span><span class="sxs-lookup"><span data-stu-id="280af-117">settings</span></span>|<span data-ttu-id="280af-118">4</span><span class="sxs-lookup"><span data-stu-id="280af-118">4</span></span>|<span data-ttu-id="280af-119">キーのグループの設定と、チーム内のすべての設定をコピーします。</span><span class="sxs-lookup"><span data-stu-id="280af-119">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="280af-120">チャンネル</span><span class="sxs-lookup"><span data-stu-id="280af-120">channels</span></span>|<span data-ttu-id="280af-121">8</span><span class="sxs-lookup"><span data-stu-id="280af-121">8</span></span>|<span data-ttu-id="280af-122">チャネルの構造 (ただし、チャネル内のメッセージではない) をコピーします。</span><span class="sxs-lookup"><span data-stu-id="280af-122">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="280af-123">メンバー</span><span class="sxs-lookup"><span data-stu-id="280af-123">members</span></span>|<span data-ttu-id="280af-124">16</span><span class="sxs-lookup"><span data-stu-id="280af-124">16</span></span>|<span data-ttu-id="280af-125">メンバーとチームの所有者にコピーします。</span><span class="sxs-lookup"><span data-stu-id="280af-125">copies the members and owners of the team.</span></span>|
