---
title: メンバー
description: TeamsApp の現在のインストール状態を説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ca42b56e2c374dbaea1df676e3a84569b192e78c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937174"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="10b4d-103">teamsAppInstalledState 列挙型</span><span class="sxs-lookup"><span data-stu-id="10b4d-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="10b4d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="10b4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10b4d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10b4d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="10b4d-106">の[teamsApp](teamsapp.md)の現在のインストール状態を説明します。</span><span class="sxs-lookup"><span data-stu-id="10b4d-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="10b4d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="10b4d-107">Members</span></span>

| <span data-ttu-id="10b4d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="10b4d-108">Member</span></span> | <span data-ttu-id="10b4d-109">値</span><span class="sxs-lookup"><span data-stu-id="10b4d-109">Value</span></span>| <span data-ttu-id="10b4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="10b4d-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="10b4d-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="10b4d-111">notInstalled</span></span>|<span data-ttu-id="10b4d-112">0</span><span class="sxs-lookup"><span data-stu-id="10b4d-112">0</span></span>|<span data-ttu-id="10b4d-113">チームには、アプリケーションはインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="10b4d-113">App is not installed to team.</span></span>|
|<span data-ttu-id="10b4d-114">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="10b4d-114">installed</span></span>|<span data-ttu-id="10b4d-115">1</span><span class="sxs-lookup"><span data-stu-id="10b4d-115">1</span></span>|<span data-ttu-id="10b4d-116">アプリケーションが正常にインストールします。</span><span class="sxs-lookup"><span data-stu-id="10b4d-116">App is installed normally.</span></span>|
|<span data-ttu-id="10b4d-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="10b4d-117">installedAndHidden</span></span>|<span data-ttu-id="10b4d-118">2</span><span class="sxs-lookup"><span data-stu-id="10b4d-118">2</span></span>|<span data-ttu-id="10b4d-119">アプリケーションがインストールされているがビューから非表示にします。</span><span class="sxs-lookup"><span data-stu-id="10b4d-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="10b4d-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="10b4d-120">installedAndPermanent</span></span>|<span data-ttu-id="10b4d-121">3</span><span class="sxs-lookup"><span data-stu-id="10b4d-121">3</span></span>|<span data-ttu-id="10b4d-122">アプリケーションが完全にインストールされているしは削除できません。</span><span class="sxs-lookup"><span data-stu-id="10b4d-122">App is permanently installed and may not be removed.</span></span>|
