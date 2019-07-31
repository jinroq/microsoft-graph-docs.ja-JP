---
title: deviceGuardVirtualizationBasedSecurityState 列挙型
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1dee315f7c81df22af296a7abcd537596d1bccae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968459"
---
# <a name="deviceguardvirtualizationbasedsecuritystate-enum-type"></a><span data-ttu-id="1cb95-103">deviceGuardVirtualizationBasedSecurityState 列挙型</span><span class="sxs-lookup"><span data-stu-id="1cb95-103">deviceGuardVirtualizationBasedSecurityState enum type</span></span>

> <span data-ttu-id="1cb95-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cb95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cb95-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1cb95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cb95-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1cb95-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="1cb95-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1cb95-107">Members</span></span>
|<span data-ttu-id="1cb95-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1cb95-108">Member</span></span>|<span data-ttu-id="1cb95-109">値</span><span class="sxs-lookup"><span data-stu-id="1cb95-109">Value</span></span>|<span data-ttu-id="1cb95-110">説明</span><span class="sxs-lookup"><span data-stu-id="1cb95-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cb95-111">起動</span><span class="sxs-lookup"><span data-stu-id="1cb95-111">running</span></span>|<span data-ttu-id="1cb95-112">.0</span><span class="sxs-lookup"><span data-stu-id="1cb95-112">0</span></span>|<span data-ttu-id="1cb95-113">実行中</span><span class="sxs-lookup"><span data-stu-id="1cb95-113">Running</span></span>|
|<span data-ttu-id="1cb95-114">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="1cb95-114">rebootRequired</span></span>|<span data-ttu-id="1cb95-115">1-d</span><span class="sxs-lookup"><span data-stu-id="1cb95-115">1</span></span>|<span data-ttu-id="1cb95-116">必要なルート</span><span class="sxs-lookup"><span data-stu-id="1cb95-116">Root required</span></span>|
|<span data-ttu-id="1cb95-117">require64BitArchitecture</span><span class="sxs-lookup"><span data-stu-id="1cb95-117">require64BitArchitecture</span></span>|<span data-ttu-id="1cb95-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="1cb95-118">2</span></span>|<span data-ttu-id="1cb95-119">64ビットアーキテクチャが必要</span><span class="sxs-lookup"><span data-stu-id="1cb95-119">64 bit architecture required</span></span>|
|<span data-ttu-id="1cb95-120">notLicensed</span><span class="sxs-lookup"><span data-stu-id="1cb95-120">notLicensed</span></span>|<span data-ttu-id="1cb95-121">1/3</span><span class="sxs-lookup"><span data-stu-id="1cb95-121">3</span></span>|<span data-ttu-id="1cb95-122">ライセンスなし</span><span class="sxs-lookup"><span data-stu-id="1cb95-122">Not licensed</span></span>|
|<span data-ttu-id="1cb95-123">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1cb95-123">notConfigured</span></span>|<span data-ttu-id="1cb95-124">2/4</span><span class="sxs-lookup"><span data-stu-id="1cb95-124">4</span></span>|<span data-ttu-id="1cb95-125">未構成</span><span class="sxs-lookup"><span data-stu-id="1cb95-125">Not configured</span></span>|
|<span data-ttu-id="1cb95-126">doesNotMeetHardwareRequirements</span><span class="sxs-lookup"><span data-stu-id="1cb95-126">doesNotMeetHardwareRequirements</span></span>|<span data-ttu-id="1cb95-127">5</span><span class="sxs-lookup"><span data-stu-id="1cb95-127">5</span></span>|<span data-ttu-id="1cb95-128">システムがハードウェア要件を満たしていない</span><span class="sxs-lookup"><span data-stu-id="1cb95-128">System does not meet hardware requirements</span></span>|
|<span data-ttu-id="1cb95-129">も</span><span class="sxs-lookup"><span data-stu-id="1cb95-129">other</span></span>|<span data-ttu-id="1cb95-130">42</span><span class="sxs-lookup"><span data-stu-id="1cb95-130">42</span></span>|<span data-ttu-id="1cb95-131">も.</span><span class="sxs-lookup"><span data-stu-id="1cb95-131">Other.</span></span> <span data-ttu-id="1cb95-132">Microsoft-DeviceGuard のイベントログには、詳細が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cb95-132">Event logs in microsoft-Windows-DeviceGuard have more details.</span></span>|





