---
title: securityBaselineComplianceState 列挙型
description: セキュリティベースラインコンプライアンスの状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 986484674e2a9ce5a432f18046f9a3ccd5bd1854
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943362"
---
# <a name="securitybaselinecompliancestate-enum-type"></a><span data-ttu-id="34564-103">securityBaselineComplianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="34564-103">securityBaselineComplianceState enum type</span></span>

> <span data-ttu-id="34564-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34564-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="34564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34564-106">セキュリティベースラインコンプライアンスの状態</span><span class="sxs-lookup"><span data-stu-id="34564-106">Security Baseline Compliance State</span></span>

## <a name="members"></a><span data-ttu-id="34564-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="34564-107">Members</span></span>
|<span data-ttu-id="34564-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="34564-108">Member</span></span>|<span data-ttu-id="34564-109">値</span><span class="sxs-lookup"><span data-stu-id="34564-109">Value</span></span>|<span data-ttu-id="34564-110">説明</span><span class="sxs-lookup"><span data-stu-id="34564-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34564-111">不明</span><span class="sxs-lookup"><span data-stu-id="34564-111">unknown</span></span>|<span data-ttu-id="34564-112">.0</span><span class="sxs-lookup"><span data-stu-id="34564-112">0</span></span>|<span data-ttu-id="34564-113">不明な状態</span><span class="sxs-lookup"><span data-stu-id="34564-113">Unknown state</span></span>|
|<span data-ttu-id="34564-114">な</span><span class="sxs-lookup"><span data-stu-id="34564-114">secure</span></span>|<span data-ttu-id="34564-115">1-d</span><span class="sxs-lookup"><span data-stu-id="34564-115">1</span></span>|<span data-ttu-id="34564-116">セキュリティで保護された状態</span><span class="sxs-lookup"><span data-stu-id="34564-116">Secure state</span></span>|
|<span data-ttu-id="34564-117">notApplicable</span><span class="sxs-lookup"><span data-stu-id="34564-117">notApplicable</span></span>|<span data-ttu-id="34564-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="34564-118">2</span></span>|<span data-ttu-id="34564-119">該当なしの状態</span><span class="sxs-lookup"><span data-stu-id="34564-119">Not applicable state</span></span>|
|<span data-ttu-id="34564-120">notSecure</span><span class="sxs-lookup"><span data-stu-id="34564-120">notSecure</span></span>|<span data-ttu-id="34564-121">1/3</span><span class="sxs-lookup"><span data-stu-id="34564-121">3</span></span>|<span data-ttu-id="34564-122">セキュリティで保護されていない状態</span><span class="sxs-lookup"><span data-stu-id="34564-122">Not secure state</span></span>|
|<span data-ttu-id="34564-123">error</span><span class="sxs-lookup"><span data-stu-id="34564-123">error</span></span>|<span data-ttu-id="34564-124">2/4</span><span class="sxs-lookup"><span data-stu-id="34564-124">4</span></span>|<span data-ttu-id="34564-125">エラー状態</span><span class="sxs-lookup"><span data-stu-id="34564-125">Error state</span></span>|
|<span data-ttu-id="34564-126">異なる</span><span class="sxs-lookup"><span data-stu-id="34564-126">conflict</span></span>|<span data-ttu-id="34564-127">5</span><span class="sxs-lookup"><span data-stu-id="34564-127">5</span></span>|<span data-ttu-id="34564-128">競合状態</span><span class="sxs-lookup"><span data-stu-id="34564-128">Conflict state</span></span>|




