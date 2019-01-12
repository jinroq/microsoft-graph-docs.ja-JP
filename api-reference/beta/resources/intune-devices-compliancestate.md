---
title: complianceState 列挙型
description: コンプライアンス状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8936d2116a3aaa8e77905174b46a3997c317cfda
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968716"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="42ada-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="42ada-103">complianceState enum type</span></span>

> <span data-ttu-id="42ada-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42ada-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42ada-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42ada-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42ada-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="42ada-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42ada-107">コンプライアンス状態です。</span><span class="sxs-lookup"><span data-stu-id="42ada-107">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="42ada-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="42ada-108">Members</span></span>
|<span data-ttu-id="42ada-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="42ada-109">Member</span></span>|<span data-ttu-id="42ada-110">値</span><span class="sxs-lookup"><span data-stu-id="42ada-110">Value</span></span>|<span data-ttu-id="42ada-111">説明</span><span class="sxs-lookup"><span data-stu-id="42ada-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42ada-112">不明</span><span class="sxs-lookup"><span data-stu-id="42ada-112">unknown</span></span>|<span data-ttu-id="42ada-113">0</span><span class="sxs-lookup"><span data-stu-id="42ada-113">0</span></span>|<span data-ttu-id="42ada-114">不明。</span><span class="sxs-lookup"><span data-stu-id="42ada-114">Unknown.</span></span>|
|<span data-ttu-id="42ada-115">準拠</span><span class="sxs-lookup"><span data-stu-id="42ada-115">compliant</span></span>|<span data-ttu-id="42ada-116">1</span><span class="sxs-lookup"><span data-stu-id="42ada-116">1</span></span>|<span data-ttu-id="42ada-117">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="42ada-117">Compliant.</span></span>|
|<span data-ttu-id="42ada-118">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="42ada-118">noncompliant</span></span>|<span data-ttu-id="42ada-119">2</span><span class="sxs-lookup"><span data-stu-id="42ada-119">2</span></span>|<span data-ttu-id="42ada-120">デバイスは非準拠、企業のリソースがブロックされました。</span><span class="sxs-lookup"><span data-stu-id="42ada-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="42ada-121">競合</span><span class="sxs-lookup"><span data-stu-id="42ada-121">conflict</span></span>|<span data-ttu-id="42ada-122">3</span><span class="sxs-lookup"><span data-stu-id="42ada-122">3</span></span>|<span data-ttu-id="42ada-123">その他の規則と競合しています。</span><span class="sxs-lookup"><span data-stu-id="42ada-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="42ada-124">エラー</span><span class="sxs-lookup"><span data-stu-id="42ada-124">error</span></span>|<span data-ttu-id="42ada-125">4</span><span class="sxs-lookup"><span data-stu-id="42ada-125">4</span></span>|<span data-ttu-id="42ada-126">エラー。</span><span class="sxs-lookup"><span data-stu-id="42ada-126">Error.</span></span>|
|<span data-ttu-id="42ada-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="42ada-127">inGracePeriod</span></span>|<span data-ttu-id="42ada-128">254</span><span class="sxs-lookup"><span data-stu-id="42ada-128">254</span></span>|<span data-ttu-id="42ada-129">デバイスは非準拠ですが、社内リソースへのアクセスにはまだ</span><span class="sxs-lookup"><span data-stu-id="42ada-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="42ada-130">configManager</span><span class="sxs-lookup"><span data-stu-id="42ada-130">configManager</span></span>|<span data-ttu-id="42ada-131">255</span><span class="sxs-lookup"><span data-stu-id="42ada-131">255</span></span>|<span data-ttu-id="42ada-132">構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="42ada-132">Managed by Config Manager</span></span>|





