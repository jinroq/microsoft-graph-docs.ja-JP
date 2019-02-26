---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d578417c616fc2dbf30b8fe95d2f58ede5fd3df2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253359"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="ebd1d-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="ebd1d-103">complianceState enum type</span></span>

> <span data-ttu-id="ebd1d-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebd1d-105">コンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="ebd1d-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ebd1d-106">Members</span></span>
|<span data-ttu-id="ebd1d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ebd1d-107">Member</span></span>|<span data-ttu-id="ebd1d-108">値</span><span class="sxs-lookup"><span data-stu-id="ebd1d-108">Value</span></span>|<span data-ttu-id="ebd1d-109">説明</span><span class="sxs-lookup"><span data-stu-id="ebd1d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd1d-110">不明</span><span class="sxs-lookup"><span data-stu-id="ebd1d-110">unknown</span></span>|<span data-ttu-id="ebd1d-111">.0</span><span class="sxs-lookup"><span data-stu-id="ebd1d-111">0</span></span>|<span data-ttu-id="ebd1d-112">わかり.</span><span class="sxs-lookup"><span data-stu-id="ebd1d-112">Unknown.</span></span>|
|<span data-ttu-id="ebd1d-113">要件</span><span class="sxs-lookup"><span data-stu-id="ebd1d-113">compliant</span></span>|<span data-ttu-id="ebd1d-114">1-d</span><span class="sxs-lookup"><span data-stu-id="ebd1d-114">1</span></span>|<span data-ttu-id="ebd1d-115">要件.</span><span class="sxs-lookup"><span data-stu-id="ebd1d-115">Compliant.</span></span>|
|<span data-ttu-id="ebd1d-116">互換性</span><span class="sxs-lookup"><span data-stu-id="ebd1d-116">noncompliant</span></span>|<span data-ttu-id="ebd1d-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ebd1d-117">2</span></span>|<span data-ttu-id="ebd1d-118">デバイスは非準拠で、企業リソースからブロックされます。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="ebd1d-119">異なる</span><span class="sxs-lookup"><span data-stu-id="ebd1d-119">conflict</span></span>|<span data-ttu-id="ebd1d-120">1/3</span><span class="sxs-lookup"><span data-stu-id="ebd1d-120">3</span></span>|<span data-ttu-id="ebd1d-121">他のルールと競合しています。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="ebd1d-122">エラー</span><span class="sxs-lookup"><span data-stu-id="ebd1d-122">error</span></span>|<span data-ttu-id="ebd1d-123">2/4</span><span class="sxs-lookup"><span data-stu-id="ebd1d-123">4</span></span>|<span data-ttu-id="ebd1d-124">エラー。</span><span class="sxs-lookup"><span data-stu-id="ebd1d-124">Error.</span></span>|
|<span data-ttu-id="ebd1d-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="ebd1d-125">inGracePeriod</span></span>|<span data-ttu-id="ebd1d-126">254</span><span class="sxs-lookup"><span data-stu-id="ebd1d-126">254</span></span>|<span data-ttu-id="ebd1d-127">デバイスは準拠していないが、会社のリソースにアクセスできる</span><span class="sxs-lookup"><span data-stu-id="ebd1d-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="ebd1d-128">configmanager</span><span class="sxs-lookup"><span data-stu-id="ebd1d-128">configManager</span></span>|<span data-ttu-id="ebd1d-129">255</span><span class="sxs-lookup"><span data-stu-id="ebd1d-129">255</span></span>|<span data-ttu-id="ebd1d-130">構成マネージャーによる管理</span><span class="sxs-lookup"><span data-stu-id="ebd1d-130">Managed by Config Manager</span></span>|



