---
title: clonableTeamParts 列挙型
description: 'チームのどの部分のクローンを作成する必要があるについて説明します。 '
ms.openlocfilehash: 123cdb5ff7fd4a4291df5d9352b0db466908cc3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067813"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="54aab-103">clonableTeamParts 列挙型</span><span class="sxs-lookup"><span data-stu-id="54aab-103">clonableTeamParts enum type</span></span>

> <span data-ttu-id="54aab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54aab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54aab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54aab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54aab-106">[チーム](../resources/team.md)のどの部分のクローンを作成する必要があるについて説明します。</span><span class="sxs-lookup"><span data-stu-id="54aab-106">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="54aab-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="54aab-107">Members</span></span>

| <span data-ttu-id="54aab-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="54aab-108">Member</span></span> | <span data-ttu-id="54aab-109">値</span><span class="sxs-lookup"><span data-stu-id="54aab-109">Value</span></span>| <span data-ttu-id="54aab-110">説明</span><span class="sxs-lookup"><span data-stu-id="54aab-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="54aab-111">apps</span><span class="sxs-lookup"><span data-stu-id="54aab-111">apps</span></span>|<span data-ttu-id="54aab-112">1</span><span class="sxs-lookup"><span data-stu-id="54aab-112">1</span></span>|<span data-ttu-id="54aab-113">インストールされたアプリの一覧をコピーします。</span><span class="sxs-lookup"><span data-stu-id="54aab-113">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="54aab-114">タブ</span><span class="sxs-lookup"><span data-stu-id="54aab-114">tabs</span></span>|<span data-ttu-id="54aab-115">2</span><span class="sxs-lookup"><span data-stu-id="54aab-115">2</span></span>|<span data-ttu-id="54aab-116">チャネル内のタブにコピーします。</span><span class="sxs-lookup"><span data-stu-id="54aab-116">copies the tabs within channels.</span></span>|
|<span data-ttu-id="54aab-117">settings</span><span class="sxs-lookup"><span data-stu-id="54aab-117">settings</span></span>|<span data-ttu-id="54aab-118">4</span><span class="sxs-lookup"><span data-stu-id="54aab-118">4</span></span>|<span data-ttu-id="54aab-119">キーのグループの設定と、チーム内のすべての設定をコピーします。</span><span class="sxs-lookup"><span data-stu-id="54aab-119">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="54aab-120">チャンネル</span><span class="sxs-lookup"><span data-stu-id="54aab-120">channels</span></span>|<span data-ttu-id="54aab-121">8</span><span class="sxs-lookup"><span data-stu-id="54aab-121">8</span></span>|<span data-ttu-id="54aab-122">チャネルの構造 (ただし、チャネル内のメッセージではない) をコピーします。</span><span class="sxs-lookup"><span data-stu-id="54aab-122">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="54aab-123">メンバー</span><span class="sxs-lookup"><span data-stu-id="54aab-123">members</span></span>|<span data-ttu-id="54aab-124">16</span><span class="sxs-lookup"><span data-stu-id="54aab-124">16</span></span>|<span data-ttu-id="54aab-125">メンバーとチームの所有者にコピーします。</span><span class="sxs-lookup"><span data-stu-id="54aab-125">copies the members and owners of the team.</span></span>|
