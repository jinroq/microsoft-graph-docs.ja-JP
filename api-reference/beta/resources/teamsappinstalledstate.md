---
title: メンバー
description: TeamsApp の現在のインストール状態を説明します。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4e453a28b0c3ebc2957cf7e1a92a846e8e4758e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847573"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="18e96-103">teamsAppInstalledState 列挙型</span><span class="sxs-lookup"><span data-stu-id="18e96-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="18e96-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18e96-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18e96-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18e96-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18e96-106">の[teamsApp](teamsapp.md)の現在のインストール状態を説明します。</span><span class="sxs-lookup"><span data-stu-id="18e96-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="18e96-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="18e96-107">Members</span></span>

| <span data-ttu-id="18e96-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="18e96-108">Member</span></span> | <span data-ttu-id="18e96-109">値</span><span class="sxs-lookup"><span data-stu-id="18e96-109">Value</span></span>| <span data-ttu-id="18e96-110">説明</span><span class="sxs-lookup"><span data-stu-id="18e96-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="18e96-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="18e96-111">notInstalled</span></span>|<span data-ttu-id="18e96-112">0</span><span class="sxs-lookup"><span data-stu-id="18e96-112">0</span></span>|<span data-ttu-id="18e96-113">チームには、アプリケーションはインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="18e96-113">App is not installed to team.</span></span>|
|<span data-ttu-id="18e96-114">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="18e96-114">installed</span></span>|<span data-ttu-id="18e96-115">1</span><span class="sxs-lookup"><span data-stu-id="18e96-115">1</span></span>|<span data-ttu-id="18e96-116">アプリケーションが正常にインストールします。</span><span class="sxs-lookup"><span data-stu-id="18e96-116">App is installed normally.</span></span>|
|<span data-ttu-id="18e96-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="18e96-117">installedAndHidden</span></span>|<span data-ttu-id="18e96-118">2</span><span class="sxs-lookup"><span data-stu-id="18e96-118">2</span></span>|<span data-ttu-id="18e96-119">アプリケーションがインストールされているがビューから非表示にします。</span><span class="sxs-lookup"><span data-stu-id="18e96-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="18e96-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="18e96-120">installedAndPermanent</span></span>|<span data-ttu-id="18e96-121">3</span><span class="sxs-lookup"><span data-stu-id="18e96-121">3</span></span>|<span data-ttu-id="18e96-122">アプリケーションが完全にインストールされているしは削除できません。</span><span class="sxs-lookup"><span data-stu-id="18e96-122">App is permanently installed and may not be removed.</span></span>|
