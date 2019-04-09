---
title: securityBaselineComplianceState 列挙型
description: セキュリティベースラインコンプライアンスの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c5503c957b54393b66ecfb5ec487cfe059d1d4f
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524478"
---
# <a name="securitybaselinecompliancestate-enum-type"></a><span data-ttu-id="8a4b9-103">securityBaselineComplianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="8a4b9-103">securityBaselineComplianceState enum type</span></span>

> <span data-ttu-id="8a4b9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a4b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a4b9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a4b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a4b9-106">セキュリティベースラインコンプライアンスの状態</span><span class="sxs-lookup"><span data-stu-id="8a4b9-106">Security Baseline Compliance State</span></span>

## <a name="members"></a><span data-ttu-id="8a4b9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a4b9-107">Members</span></span>
|<span data-ttu-id="8a4b9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a4b9-108">Member</span></span>|<span data-ttu-id="8a4b9-109">値</span><span class="sxs-lookup"><span data-stu-id="8a4b9-109">Value</span></span>|<span data-ttu-id="8a4b9-110">説明</span><span class="sxs-lookup"><span data-stu-id="8a4b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a4b9-111">不明</span><span class="sxs-lookup"><span data-stu-id="8a4b9-111">unknown</span></span>|<span data-ttu-id="8a4b9-112">.0</span><span class="sxs-lookup"><span data-stu-id="8a4b9-112">0</span></span>|<span data-ttu-id="8a4b9-113">不明な状態</span><span class="sxs-lookup"><span data-stu-id="8a4b9-113">Unknown state</span></span>|
|<span data-ttu-id="8a4b9-114">な</span><span class="sxs-lookup"><span data-stu-id="8a4b9-114">secure</span></span>|<span data-ttu-id="8a4b9-115">1</span><span class="sxs-lookup"><span data-stu-id="8a4b9-115">1</span></span>|<span data-ttu-id="8a4b9-116">セキュリティで保護された状態</span><span class="sxs-lookup"><span data-stu-id="8a4b9-116">Secure state</span></span>|
|<span data-ttu-id="8a4b9-117">notapplicable</span><span class="sxs-lookup"><span data-stu-id="8a4b9-117">notApplicable</span></span>|<span data-ttu-id="8a4b9-118">2</span><span class="sxs-lookup"><span data-stu-id="8a4b9-118">2</span></span>|<span data-ttu-id="8a4b9-119">該当なしの状態</span><span class="sxs-lookup"><span data-stu-id="8a4b9-119">Not applicable state</span></span>|
|<span data-ttu-id="8a4b9-120">notsecure</span><span class="sxs-lookup"><span data-stu-id="8a4b9-120">notSecure</span></span>|<span data-ttu-id="8a4b9-121">1/3</span><span class="sxs-lookup"><span data-stu-id="8a4b9-121">3</span></span>|<span data-ttu-id="8a4b9-122">セキュリティで保護されていない状態</span><span class="sxs-lookup"><span data-stu-id="8a4b9-122">Not secure state</span></span>|
|<span data-ttu-id="8a4b9-123">エラー</span><span class="sxs-lookup"><span data-stu-id="8a4b9-123">error</span></span>|<span data-ttu-id="8a4b9-124">2/4</span><span class="sxs-lookup"><span data-stu-id="8a4b9-124">4</span></span>|<span data-ttu-id="8a4b9-125">エラー状態</span><span class="sxs-lookup"><span data-stu-id="8a4b9-125">Error state</span></span>|
|<span data-ttu-id="8a4b9-126">異なる</span><span class="sxs-lookup"><span data-stu-id="8a4b9-126">conflict</span></span>|<span data-ttu-id="8a4b9-127">5</span><span class="sxs-lookup"><span data-stu-id="8a4b9-127">5</span></span>|<span data-ttu-id="8a4b9-128">競合状態</span><span class="sxs-lookup"><span data-stu-id="8a4b9-128">Conflict state</span></span>|







