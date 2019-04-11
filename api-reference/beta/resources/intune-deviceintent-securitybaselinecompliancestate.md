---
title: securityBaselineComplianceState 列挙型
description: セキュリティベースラインコンプライアンスの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bec545efcc5c2558f0a882781a475444a644a940
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807533"
---
# <a name="securitybaselinecompliancestate-enum-type"></a><span data-ttu-id="e2525-103">securityBaselineComplianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e2525-103">securityBaselineComplianceState enum type</span></span>

> <span data-ttu-id="e2525-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2525-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2525-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2525-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2525-106">セキュリティベースラインコンプライアンスの状態</span><span class="sxs-lookup"><span data-stu-id="e2525-106">Security Baseline Compliance State</span></span>

## <a name="members"></a><span data-ttu-id="e2525-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e2525-107">Members</span></span>
|<span data-ttu-id="e2525-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e2525-108">Member</span></span>|<span data-ttu-id="e2525-109">値</span><span class="sxs-lookup"><span data-stu-id="e2525-109">Value</span></span>|<span data-ttu-id="e2525-110">説明</span><span class="sxs-lookup"><span data-stu-id="e2525-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2525-111">不明</span><span class="sxs-lookup"><span data-stu-id="e2525-111">unknown</span></span>|<span data-ttu-id="e2525-112">.0</span><span class="sxs-lookup"><span data-stu-id="e2525-112">0</span></span>|<span data-ttu-id="e2525-113">不明な状態</span><span class="sxs-lookup"><span data-stu-id="e2525-113">Unknown state</span></span>|
|<span data-ttu-id="e2525-114">な</span><span class="sxs-lookup"><span data-stu-id="e2525-114">secure</span></span>|<span data-ttu-id="e2525-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e2525-115">1</span></span>|<span data-ttu-id="e2525-116">セキュリティで保護された状態</span><span class="sxs-lookup"><span data-stu-id="e2525-116">Secure state</span></span>|
|<span data-ttu-id="e2525-117">notapplicable</span><span class="sxs-lookup"><span data-stu-id="e2525-117">notApplicable</span></span>|<span data-ttu-id="e2525-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e2525-118">2</span></span>|<span data-ttu-id="e2525-119">該当なしの状態</span><span class="sxs-lookup"><span data-stu-id="e2525-119">Not applicable state</span></span>|
|<span data-ttu-id="e2525-120">notsecure</span><span class="sxs-lookup"><span data-stu-id="e2525-120">notSecure</span></span>|<span data-ttu-id="e2525-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e2525-121">3</span></span>|<span data-ttu-id="e2525-122">セキュリティで保護されていない状態</span><span class="sxs-lookup"><span data-stu-id="e2525-122">Not secure state</span></span>|
|<span data-ttu-id="e2525-123">エラー</span><span class="sxs-lookup"><span data-stu-id="e2525-123">error</span></span>|<span data-ttu-id="e2525-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e2525-124">4</span></span>|<span data-ttu-id="e2525-125">エラー状態</span><span class="sxs-lookup"><span data-stu-id="e2525-125">Error state</span></span>|
|<span data-ttu-id="e2525-126">異なる</span><span class="sxs-lookup"><span data-stu-id="e2525-126">conflict</span></span>|<span data-ttu-id="e2525-127">5</span><span class="sxs-lookup"><span data-stu-id="e2525-127">5</span></span>|<span data-ttu-id="e2525-128">競合状態</span><span class="sxs-lookup"><span data-stu-id="e2525-128">Conflict state</span></span>|





