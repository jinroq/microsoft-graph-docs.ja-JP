---
title: securityBaselineComplianceState 列挙型
description: セキュリティベースラインコンプライアンスの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bec545efcc5c2558f0a882781a475444a644a940
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550680"
---
# <a name="securitybaselinecompliancestate-enum-type"></a><span data-ttu-id="19fd4-103">securityBaselineComplianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="19fd4-103">securityBaselineComplianceState enum type</span></span>

> <span data-ttu-id="19fd4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19fd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19fd4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="19fd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19fd4-106">セキュリティベースラインコンプライアンスの状態</span><span class="sxs-lookup"><span data-stu-id="19fd4-106">Security Baseline Compliance State</span></span>

## <a name="members"></a><span data-ttu-id="19fd4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="19fd4-107">Members</span></span>
|<span data-ttu-id="19fd4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="19fd4-108">Member</span></span>|<span data-ttu-id="19fd4-109">値</span><span class="sxs-lookup"><span data-stu-id="19fd4-109">Value</span></span>|<span data-ttu-id="19fd4-110">説明</span><span class="sxs-lookup"><span data-stu-id="19fd4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19fd4-111">不明</span><span class="sxs-lookup"><span data-stu-id="19fd4-111">unknown</span></span>|<span data-ttu-id="19fd4-112">.0</span><span class="sxs-lookup"><span data-stu-id="19fd4-112">0</span></span>|<span data-ttu-id="19fd4-113">不明な状態</span><span class="sxs-lookup"><span data-stu-id="19fd4-113">Unknown state</span></span>|
|<span data-ttu-id="19fd4-114">な</span><span class="sxs-lookup"><span data-stu-id="19fd4-114">secure</span></span>|<span data-ttu-id="19fd4-115">1 </span><span class="sxs-lookup"><span data-stu-id="19fd4-115">1</span></span>|<span data-ttu-id="19fd4-116">セキュリティで保護された状態</span><span class="sxs-lookup"><span data-stu-id="19fd4-116">Secure state</span></span>|
|<span data-ttu-id="19fd4-117">notapplicable</span><span class="sxs-lookup"><span data-stu-id="19fd4-117">notApplicable</span></span>|<span data-ttu-id="19fd4-118">2 </span><span class="sxs-lookup"><span data-stu-id="19fd4-118">2</span></span>|<span data-ttu-id="19fd4-119">該当なしの状態</span><span class="sxs-lookup"><span data-stu-id="19fd4-119">Not applicable state</span></span>|
|<span data-ttu-id="19fd4-120">notsecure</span><span class="sxs-lookup"><span data-stu-id="19fd4-120">notSecure</span></span>|<span data-ttu-id="19fd4-121">3 </span><span class="sxs-lookup"><span data-stu-id="19fd4-121">3</span></span>|<span data-ttu-id="19fd4-122">セキュリティで保護されていない状態</span><span class="sxs-lookup"><span data-stu-id="19fd4-122">Not secure state</span></span>|
|<span data-ttu-id="19fd4-123">error</span><span class="sxs-lookup"><span data-stu-id="19fd4-123">error</span></span>|<span data-ttu-id="19fd4-124">4 </span><span class="sxs-lookup"><span data-stu-id="19fd4-124">4</span></span>|<span data-ttu-id="19fd4-125">エラー状態</span><span class="sxs-lookup"><span data-stu-id="19fd4-125">Error state</span></span>|
|<span data-ttu-id="19fd4-126">異なる</span><span class="sxs-lookup"><span data-stu-id="19fd4-126">conflict</span></span>|<span data-ttu-id="19fd4-127">5 </span><span class="sxs-lookup"><span data-stu-id="19fd4-127">5</span></span>|<span data-ttu-id="19fd4-128">競合状態</span><span class="sxs-lookup"><span data-stu-id="19fd4-128">Conflict state</span></span>|





