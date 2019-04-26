---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d578417c616fc2dbf30b8fe95d2f58ede5fd3df2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568139"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="1ebf8-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="1ebf8-103">complianceState enum type</span></span>

> <span data-ttu-id="1ebf8-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1ebf8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ebf8-105">コンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="1ebf8-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="1ebf8-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1ebf8-106">Members</span></span>
|<span data-ttu-id="1ebf8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1ebf8-107">Member</span></span>|<span data-ttu-id="1ebf8-108">値</span><span class="sxs-lookup"><span data-stu-id="1ebf8-108">Value</span></span>|<span data-ttu-id="1ebf8-109">説明</span><span class="sxs-lookup"><span data-stu-id="1ebf8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ebf8-110">不明</span><span class="sxs-lookup"><span data-stu-id="1ebf8-110">unknown</span></span>|<span data-ttu-id="1ebf8-111">.0</span><span class="sxs-lookup"><span data-stu-id="1ebf8-111">0</span></span>|<span data-ttu-id="1ebf8-112">わかり.</span><span class="sxs-lookup"><span data-stu-id="1ebf8-112">Unknown.</span></span>|
|<span data-ttu-id="1ebf8-113">要件</span><span class="sxs-lookup"><span data-stu-id="1ebf8-113">compliant</span></span>|<span data-ttu-id="1ebf8-114">1 </span><span class="sxs-lookup"><span data-stu-id="1ebf8-114">1</span></span>|<span data-ttu-id="1ebf8-115">要件.</span><span class="sxs-lookup"><span data-stu-id="1ebf8-115">Compliant.</span></span>|
|<span data-ttu-id="1ebf8-116">互換性</span><span class="sxs-lookup"><span data-stu-id="1ebf8-116">noncompliant</span></span>|<span data-ttu-id="1ebf8-117">2 </span><span class="sxs-lookup"><span data-stu-id="1ebf8-117">2</span></span>|<span data-ttu-id="1ebf8-118">デバイスは非準拠で、企業リソースからブロックされます。</span><span class="sxs-lookup"><span data-stu-id="1ebf8-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="1ebf8-119">異なる</span><span class="sxs-lookup"><span data-stu-id="1ebf8-119">conflict</span></span>|<span data-ttu-id="1ebf8-120">3 </span><span class="sxs-lookup"><span data-stu-id="1ebf8-120">3</span></span>|<span data-ttu-id="1ebf8-121">他のルールと競合しています。</span><span class="sxs-lookup"><span data-stu-id="1ebf8-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="1ebf8-122">error</span><span class="sxs-lookup"><span data-stu-id="1ebf8-122">error</span></span>|<span data-ttu-id="1ebf8-123">4 </span><span class="sxs-lookup"><span data-stu-id="1ebf8-123">4</span></span>|<span data-ttu-id="1ebf8-124">Error。</span><span class="sxs-lookup"><span data-stu-id="1ebf8-124">Error.</span></span>|
|<span data-ttu-id="1ebf8-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="1ebf8-125">inGracePeriod</span></span>|<span data-ttu-id="1ebf8-126">254</span><span class="sxs-lookup"><span data-stu-id="1ebf8-126">254</span></span>|<span data-ttu-id="1ebf8-127">デバイスは準拠していないが、会社のリソースにアクセスできる</span><span class="sxs-lookup"><span data-stu-id="1ebf8-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="1ebf8-128">configmanager</span><span class="sxs-lookup"><span data-stu-id="1ebf8-128">configManager</span></span>|<span data-ttu-id="1ebf8-129">255</span><span class="sxs-lookup"><span data-stu-id="1ebf8-129">255</span></span>|<span data-ttu-id="1ebf8-130">構成マネージャーによる管理</span><span class="sxs-lookup"><span data-stu-id="1ebf8-130">Managed by Config Manager</span></span>|



