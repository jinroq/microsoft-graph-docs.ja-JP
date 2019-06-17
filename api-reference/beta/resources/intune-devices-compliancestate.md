---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83f39e4c795d57b6bb5aa5633ed481963419e041
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983289"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="e3d09-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e3d09-103">complianceState enum type</span></span>

> <span data-ttu-id="e3d09-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3d09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3d09-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3d09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3d09-106">コンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="e3d09-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="e3d09-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3d09-107">Members</span></span>
|<span data-ttu-id="e3d09-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3d09-108">Member</span></span>|<span data-ttu-id="e3d09-109">値</span><span class="sxs-lookup"><span data-stu-id="e3d09-109">Value</span></span>|<span data-ttu-id="e3d09-110">説明</span><span class="sxs-lookup"><span data-stu-id="e3d09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3d09-111">不明</span><span class="sxs-lookup"><span data-stu-id="e3d09-111">unknown</span></span>|<span data-ttu-id="e3d09-112">.0</span><span class="sxs-lookup"><span data-stu-id="e3d09-112">0</span></span>|<span data-ttu-id="e3d09-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="e3d09-113">Unknown.</span></span>|
|<span data-ttu-id="e3d09-114">要件</span><span class="sxs-lookup"><span data-stu-id="e3d09-114">compliant</span></span>|<span data-ttu-id="e3d09-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e3d09-115">1</span></span>|<span data-ttu-id="e3d09-116">要件.</span><span class="sxs-lookup"><span data-stu-id="e3d09-116">Compliant.</span></span>|
|<span data-ttu-id="e3d09-117">互換性</span><span class="sxs-lookup"><span data-stu-id="e3d09-117">noncompliant</span></span>|<span data-ttu-id="e3d09-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e3d09-118">2</span></span>|<span data-ttu-id="e3d09-119">デバイスは非準拠で、企業リソースからブロックされます。</span><span class="sxs-lookup"><span data-stu-id="e3d09-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="e3d09-120">異なる</span><span class="sxs-lookup"><span data-stu-id="e3d09-120">conflict</span></span>|<span data-ttu-id="e3d09-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e3d09-121">3</span></span>|<span data-ttu-id="e3d09-122">他のルールと競合しています。</span><span class="sxs-lookup"><span data-stu-id="e3d09-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="e3d09-123">error</span><span class="sxs-lookup"><span data-stu-id="e3d09-123">error</span></span>|<span data-ttu-id="e3d09-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e3d09-124">4</span></span>|<span data-ttu-id="e3d09-125">Error。</span><span class="sxs-lookup"><span data-stu-id="e3d09-125">Error.</span></span>|
|<span data-ttu-id="e3d09-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="e3d09-126">inGracePeriod</span></span>|<span data-ttu-id="e3d09-127">254</span><span class="sxs-lookup"><span data-stu-id="e3d09-127">254</span></span>|<span data-ttu-id="e3d09-128">デバイスは準拠していないが、会社のリソースにアクセスできる</span><span class="sxs-lookup"><span data-stu-id="e3d09-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="e3d09-129">configManager</span><span class="sxs-lookup"><span data-stu-id="e3d09-129">configManager</span></span>|<span data-ttu-id="e3d09-130">255</span><span class="sxs-lookup"><span data-stu-id="e3d09-130">255</span></span>|<span data-ttu-id="e3d09-131">構成マネージャーによる管理</span><span class="sxs-lookup"><span data-stu-id="e3d09-131">Managed by Config Manager</span></span>|





