---
title: securityBaselineComplianceState 列挙型
description: セキュリティベースラインコンプライアンスの状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ecde3520bb2fcced3687e04dd9fd89cceec2a11
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983457"
---
# <a name="securitybaselinecompliancestate-enum-type"></a><span data-ttu-id="bf34e-103">securityBaselineComplianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="bf34e-103">securityBaselineComplianceState enum type</span></span>

> <span data-ttu-id="bf34e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf34e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf34e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf34e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf34e-106">セキュリティベースラインコンプライアンスの状態</span><span class="sxs-lookup"><span data-stu-id="bf34e-106">Security Baseline Compliance State</span></span>

## <a name="members"></a><span data-ttu-id="bf34e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bf34e-107">Members</span></span>
|<span data-ttu-id="bf34e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bf34e-108">Member</span></span>|<span data-ttu-id="bf34e-109">値</span><span class="sxs-lookup"><span data-stu-id="bf34e-109">Value</span></span>|<span data-ttu-id="bf34e-110">説明</span><span class="sxs-lookup"><span data-stu-id="bf34e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf34e-111">不明</span><span class="sxs-lookup"><span data-stu-id="bf34e-111">unknown</span></span>|<span data-ttu-id="bf34e-112">.0</span><span class="sxs-lookup"><span data-stu-id="bf34e-112">0</span></span>|<span data-ttu-id="bf34e-113">不明な状態</span><span class="sxs-lookup"><span data-stu-id="bf34e-113">Unknown state</span></span>|
|<span data-ttu-id="bf34e-114">な</span><span class="sxs-lookup"><span data-stu-id="bf34e-114">secure</span></span>|<span data-ttu-id="bf34e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="bf34e-115">1</span></span>|<span data-ttu-id="bf34e-116">セキュリティで保護された状態</span><span class="sxs-lookup"><span data-stu-id="bf34e-116">Secure state</span></span>|
|<span data-ttu-id="bf34e-117">notApplicable</span><span class="sxs-lookup"><span data-stu-id="bf34e-117">notApplicable</span></span>|<span data-ttu-id="bf34e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="bf34e-118">2</span></span>|<span data-ttu-id="bf34e-119">該当なしの状態</span><span class="sxs-lookup"><span data-stu-id="bf34e-119">Not applicable state</span></span>|
|<span data-ttu-id="bf34e-120">notSecure</span><span class="sxs-lookup"><span data-stu-id="bf34e-120">notSecure</span></span>|<span data-ttu-id="bf34e-121">1/3</span><span class="sxs-lookup"><span data-stu-id="bf34e-121">3</span></span>|<span data-ttu-id="bf34e-122">セキュリティで保護されていない状態</span><span class="sxs-lookup"><span data-stu-id="bf34e-122">Not secure state</span></span>|
|<span data-ttu-id="bf34e-123">error</span><span class="sxs-lookup"><span data-stu-id="bf34e-123">error</span></span>|<span data-ttu-id="bf34e-124">2/4</span><span class="sxs-lookup"><span data-stu-id="bf34e-124">4</span></span>|<span data-ttu-id="bf34e-125">エラー状態</span><span class="sxs-lookup"><span data-stu-id="bf34e-125">Error state</span></span>|
|<span data-ttu-id="bf34e-126">異なる</span><span class="sxs-lookup"><span data-stu-id="bf34e-126">conflict</span></span>|<span data-ttu-id="bf34e-127">5</span><span class="sxs-lookup"><span data-stu-id="bf34e-127">5</span></span>|<span data-ttu-id="bf34e-128">競合状態</span><span class="sxs-lookup"><span data-stu-id="bf34e-128">Conflict state</span></span>|





