---
title: complianceState 列挙型
description: コンプライアンス状態です。
author: tfitzmac
ms.openlocfilehash: 3fa0548c2a67aa5def5f859014f52e97bdda815b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321232"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="773b9-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="773b9-103">complianceState enum type</span></span>

> <span data-ttu-id="773b9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="773b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="773b9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="773b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="773b9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="773b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="773b9-107">コンプライアンス状態です。</span><span class="sxs-lookup"><span data-stu-id="773b9-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="773b9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="773b9-108">Members</span></span>
|<span data-ttu-id="773b9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="773b9-109">Member</span></span>|<span data-ttu-id="773b9-110">値</span><span class="sxs-lookup"><span data-stu-id="773b9-110">Value</span></span>|<span data-ttu-id="773b9-111">説明</span><span class="sxs-lookup"><span data-stu-id="773b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="773b9-112">不明</span><span class="sxs-lookup"><span data-stu-id="773b9-112">unknown</span></span>|<span data-ttu-id="773b9-113">0</span><span class="sxs-lookup"><span data-stu-id="773b9-113">0</span></span>|<span data-ttu-id="773b9-114">不明。</span><span class="sxs-lookup"><span data-stu-id="773b9-114">Unknown.</span></span>|
|<span data-ttu-id="773b9-115">準拠</span><span class="sxs-lookup"><span data-stu-id="773b9-115">compliant</span></span>|<span data-ttu-id="773b9-116">1</span><span class="sxs-lookup"><span data-stu-id="773b9-116">1</span></span>|<span data-ttu-id="773b9-117">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="773b9-117">Compliant.</span></span>|
|<span data-ttu-id="773b9-118">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="773b9-118">noncompliant</span></span>|<span data-ttu-id="773b9-119">2</span><span class="sxs-lookup"><span data-stu-id="773b9-119">2</span></span>|<span data-ttu-id="773b9-120">デバイスは非準拠、企業のリソースがブロックされました。</span><span class="sxs-lookup"><span data-stu-id="773b9-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="773b9-121">競合</span><span class="sxs-lookup"><span data-stu-id="773b9-121">conflict</span></span>|<span data-ttu-id="773b9-122">3</span><span class="sxs-lookup"><span data-stu-id="773b9-122">3</span></span>|<span data-ttu-id="773b9-123">その他の規則と競合しています。</span><span class="sxs-lookup"><span data-stu-id="773b9-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="773b9-124">エラー</span><span class="sxs-lookup"><span data-stu-id="773b9-124">error</span></span>|<span data-ttu-id="773b9-125">4</span><span class="sxs-lookup"><span data-stu-id="773b9-125">4</span></span>|<span data-ttu-id="773b9-126">エラー。</span><span class="sxs-lookup"><span data-stu-id="773b9-126">Error.</span></span>|
|<span data-ttu-id="773b9-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="773b9-127">inGracePeriod</span></span>|<span data-ttu-id="773b9-128">254</span><span class="sxs-lookup"><span data-stu-id="773b9-128">254</span></span>|<span data-ttu-id="773b9-129">デバイスは非準拠ですが、社内リソースへのアクセスにはまだ</span><span class="sxs-lookup"><span data-stu-id="773b9-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="773b9-130">configManager</span><span class="sxs-lookup"><span data-stu-id="773b9-130">configManager</span></span>|<span data-ttu-id="773b9-131">255</span><span class="sxs-lookup"><span data-stu-id="773b9-131">255</span></span>|<span data-ttu-id="773b9-132">構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="773b9-132">Managed by Config Manager</span></span>|





