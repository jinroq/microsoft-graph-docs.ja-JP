---
title: complianceState 列挙型
description: コンプライアンス状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53b17f258f577e0842dbfc81c6341303f6b43799
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820343"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="2fad7-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="2fad7-103">complianceState enum type</span></span>

> <span data-ttu-id="2fad7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fad7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fad7-105">コンプライアンス状態です。</span><span class="sxs-lookup"><span data-stu-id="2fad7-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="2fad7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="2fad7-106">Members</span></span>
|<span data-ttu-id="2fad7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2fad7-107">Member</span></span>|<span data-ttu-id="2fad7-108">値</span><span class="sxs-lookup"><span data-stu-id="2fad7-108">Value</span></span>|<span data-ttu-id="2fad7-109">説明</span><span class="sxs-lookup"><span data-stu-id="2fad7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fad7-110">不明</span><span class="sxs-lookup"><span data-stu-id="2fad7-110">unknown</span></span>|<span data-ttu-id="2fad7-111">0</span><span class="sxs-lookup"><span data-stu-id="2fad7-111">0</span></span>|<span data-ttu-id="2fad7-112">不明。</span><span class="sxs-lookup"><span data-stu-id="2fad7-112">Unknown.</span></span>|
|<span data-ttu-id="2fad7-113">準拠</span><span class="sxs-lookup"><span data-stu-id="2fad7-113">compliant</span></span>|<span data-ttu-id="2fad7-114">1</span><span class="sxs-lookup"><span data-stu-id="2fad7-114">1</span></span>|<span data-ttu-id="2fad7-115">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="2fad7-115">Compliant.</span></span>|
|<span data-ttu-id="2fad7-116">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="2fad7-116">noncompliant</span></span>|<span data-ttu-id="2fad7-117">2</span><span class="sxs-lookup"><span data-stu-id="2fad7-117">2</span></span>|<span data-ttu-id="2fad7-118">デバイスは非準拠、企業のリソースがブロックされました。</span><span class="sxs-lookup"><span data-stu-id="2fad7-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="2fad7-119">競合</span><span class="sxs-lookup"><span data-stu-id="2fad7-119">conflict</span></span>|<span data-ttu-id="2fad7-120">3</span><span class="sxs-lookup"><span data-stu-id="2fad7-120">3</span></span>|<span data-ttu-id="2fad7-121">その他の規則と競合しています。</span><span class="sxs-lookup"><span data-stu-id="2fad7-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="2fad7-122">エラー</span><span class="sxs-lookup"><span data-stu-id="2fad7-122">error</span></span>|<span data-ttu-id="2fad7-123">4</span><span class="sxs-lookup"><span data-stu-id="2fad7-123">4</span></span>|<span data-ttu-id="2fad7-124">エラー。</span><span class="sxs-lookup"><span data-stu-id="2fad7-124">Error.</span></span>|
|<span data-ttu-id="2fad7-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="2fad7-125">inGracePeriod</span></span>|<span data-ttu-id="2fad7-126">254</span><span class="sxs-lookup"><span data-stu-id="2fad7-126">254</span></span>|<span data-ttu-id="2fad7-127">デバイスは非準拠ですが、社内リソースへのアクセスにはまだ</span><span class="sxs-lookup"><span data-stu-id="2fad7-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="2fad7-128">configManager</span><span class="sxs-lookup"><span data-stu-id="2fad7-128">configManager</span></span>|<span data-ttu-id="2fad7-129">255</span><span class="sxs-lookup"><span data-stu-id="2fad7-129">255</span></span>|<span data-ttu-id="2fad7-130">構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="2fad7-130">Managed by Config Manager</span></span>|



