---
title: メンバー
description: TeamsApp の現在のインストール状態を説明します。
ms.openlocfilehash: 7f358a621a25219e78e3a02ce081d07a27395d2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072338"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="c4f60-103">teamsAppInstalledState 列挙型</span><span class="sxs-lookup"><span data-stu-id="c4f60-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="c4f60-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4f60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4f60-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4f60-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4f60-106">の[teamsApp](teamsapp.md)の現在のインストール状態を説明します。</span><span class="sxs-lookup"><span data-stu-id="c4f60-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="c4f60-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4f60-107">Members</span></span>

| <span data-ttu-id="c4f60-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4f60-108">Member</span></span> | <span data-ttu-id="c4f60-109">値</span><span class="sxs-lookup"><span data-stu-id="c4f60-109">Value</span></span>| <span data-ttu-id="c4f60-110">説明</span><span class="sxs-lookup"><span data-stu-id="c4f60-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c4f60-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="c4f60-111">notInstalled</span></span>|<span data-ttu-id="c4f60-112">0</span><span class="sxs-lookup"><span data-stu-id="c4f60-112">0</span></span>|<span data-ttu-id="c4f60-113">チームには、アプリケーションはインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="c4f60-113">App is not installed to team.</span></span>|
|<span data-ttu-id="c4f60-114">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="c4f60-114">installed</span></span>|<span data-ttu-id="c4f60-115">1</span><span class="sxs-lookup"><span data-stu-id="c4f60-115">1</span></span>|<span data-ttu-id="c4f60-116">アプリケーションが正常にインストールします。</span><span class="sxs-lookup"><span data-stu-id="c4f60-116">App is installed normally.</span></span>|
|<span data-ttu-id="c4f60-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="c4f60-117">installedAndHidden</span></span>|<span data-ttu-id="c4f60-118">2</span><span class="sxs-lookup"><span data-stu-id="c4f60-118">2</span></span>|<span data-ttu-id="c4f60-119">アプリケーションがインストールされているがビューから非表示にします。</span><span class="sxs-lookup"><span data-stu-id="c4f60-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="c4f60-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="c4f60-120">installedAndPermanent</span></span>|<span data-ttu-id="c4f60-121">3</span><span class="sxs-lookup"><span data-stu-id="c4f60-121">3</span></span>|<span data-ttu-id="c4f60-122">アプリケーションが完全にインストールされているしは削除できません。</span><span class="sxs-lookup"><span data-stu-id="c4f60-122">App is permanently installed and may not be removed.</span></span>|
