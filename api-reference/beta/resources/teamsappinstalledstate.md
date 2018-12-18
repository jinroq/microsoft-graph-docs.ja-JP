---
title: Members
description: TeamsApp の現在のインストール状態を説明します。
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316794"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="6d789-103">teamsAppInstalledState 列挙型</span><span class="sxs-lookup"><span data-stu-id="6d789-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="6d789-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6d789-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d789-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d789-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d789-106">の[teamsApp](teamsapp.md)の現在のインストール状態を説明します。</span><span class="sxs-lookup"><span data-stu-id="6d789-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="6d789-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6d789-107">Members</span></span>

| <span data-ttu-id="6d789-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6d789-108">Member</span></span> | <span data-ttu-id="6d789-109">値</span><span class="sxs-lookup"><span data-stu-id="6d789-109">Value</span></span>| <span data-ttu-id="6d789-110">説明</span><span class="sxs-lookup"><span data-stu-id="6d789-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6d789-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="6d789-111">notInstalled</span></span>|<span data-ttu-id="6d789-112">0</span><span class="sxs-lookup"><span data-stu-id="6d789-112">0</span></span>|<span data-ttu-id="6d789-113">チームには、アプリケーションはインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="6d789-113">App is not installed to team.</span></span>|
|<span data-ttu-id="6d789-114">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="6d789-114">installed</span></span>|<span data-ttu-id="6d789-115">1</span><span class="sxs-lookup"><span data-stu-id="6d789-115">1</span></span>|<span data-ttu-id="6d789-116">アプリケーションが正常にインストールします。</span><span class="sxs-lookup"><span data-stu-id="6d789-116">App is installed normally.</span></span>|
|<span data-ttu-id="6d789-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="6d789-117">installedAndHidden</span></span>|<span data-ttu-id="6d789-118">2</span><span class="sxs-lookup"><span data-stu-id="6d789-118">2</span></span>|<span data-ttu-id="6d789-119">アプリケーションがインストールされているがビューから非表示にします。</span><span class="sxs-lookup"><span data-stu-id="6d789-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="6d789-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="6d789-120">installedAndPermanent</span></span>|<span data-ttu-id="6d789-121">3</span><span class="sxs-lookup"><span data-stu-id="6d789-121">3</span></span>|<span data-ttu-id="6d789-122">アプリケーションが完全にインストールされているしは削除できません。</span><span class="sxs-lookup"><span data-stu-id="6d789-122">App is permanently installed and may not be removed.</span></span>|
