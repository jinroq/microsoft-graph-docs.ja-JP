---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6dc39839754f24ae25044b0aa249d61fe2655d68
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943034"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="22d56-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="22d56-103">complianceState enum type</span></span>

> <span data-ttu-id="22d56-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22d56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22d56-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22d56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22d56-106">コンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="22d56-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="22d56-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="22d56-107">Members</span></span>
|<span data-ttu-id="22d56-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="22d56-108">Member</span></span>|<span data-ttu-id="22d56-109">値</span><span class="sxs-lookup"><span data-stu-id="22d56-109">Value</span></span>|<span data-ttu-id="22d56-110">説明</span><span class="sxs-lookup"><span data-stu-id="22d56-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22d56-111">不明</span><span class="sxs-lookup"><span data-stu-id="22d56-111">unknown</span></span>|<span data-ttu-id="22d56-112">.0</span><span class="sxs-lookup"><span data-stu-id="22d56-112">0</span></span>|<span data-ttu-id="22d56-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="22d56-113">Unknown.</span></span>|
|<span data-ttu-id="22d56-114">要件</span><span class="sxs-lookup"><span data-stu-id="22d56-114">compliant</span></span>|<span data-ttu-id="22d56-115">1-d</span><span class="sxs-lookup"><span data-stu-id="22d56-115">1</span></span>|<span data-ttu-id="22d56-116">要件.</span><span class="sxs-lookup"><span data-stu-id="22d56-116">Compliant.</span></span>|
|<span data-ttu-id="22d56-117">互換性</span><span class="sxs-lookup"><span data-stu-id="22d56-117">noncompliant</span></span>|<span data-ttu-id="22d56-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="22d56-118">2</span></span>|<span data-ttu-id="22d56-119">デバイスは非準拠で、企業リソースからブロックされます。</span><span class="sxs-lookup"><span data-stu-id="22d56-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="22d56-120">異なる</span><span class="sxs-lookup"><span data-stu-id="22d56-120">conflict</span></span>|<span data-ttu-id="22d56-121">1/3</span><span class="sxs-lookup"><span data-stu-id="22d56-121">3</span></span>|<span data-ttu-id="22d56-122">他のルールと競合しています。</span><span class="sxs-lookup"><span data-stu-id="22d56-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="22d56-123">error</span><span class="sxs-lookup"><span data-stu-id="22d56-123">error</span></span>|<span data-ttu-id="22d56-124">2/4</span><span class="sxs-lookup"><span data-stu-id="22d56-124">4</span></span>|<span data-ttu-id="22d56-125">Error。</span><span class="sxs-lookup"><span data-stu-id="22d56-125">Error.</span></span>|
|<span data-ttu-id="22d56-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="22d56-126">inGracePeriod</span></span>|<span data-ttu-id="22d56-127">254</span><span class="sxs-lookup"><span data-stu-id="22d56-127">254</span></span>|<span data-ttu-id="22d56-128">デバイスは準拠していないが、会社のリソースにアクセスできる</span><span class="sxs-lookup"><span data-stu-id="22d56-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="22d56-129">configManager</span><span class="sxs-lookup"><span data-stu-id="22d56-129">configManager</span></span>|<span data-ttu-id="22d56-130">255</span><span class="sxs-lookup"><span data-stu-id="22d56-130">255</span></span>|<span data-ttu-id="22d56-131">構成マネージャーによる管理</span><span class="sxs-lookup"><span data-stu-id="22d56-131">Managed by Config Manager</span></span>|




