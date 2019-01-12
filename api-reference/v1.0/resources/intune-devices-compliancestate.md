---
title: complianceState 列挙型
description: コンプライアンス状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4f4c359665eb1a0087f64802b5e7c829002fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940198"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="b98cb-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="b98cb-103">complianceState enum type</span></span>

> <span data-ttu-id="b98cb-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b98cb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b98cb-105">コンプライアンス状態です。</span><span class="sxs-lookup"><span data-stu-id="b98cb-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="b98cb-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="b98cb-106">Members</span></span>
|<span data-ttu-id="b98cb-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b98cb-107">Member</span></span>|<span data-ttu-id="b98cb-108">値</span><span class="sxs-lookup"><span data-stu-id="b98cb-108">Value</span></span>|<span data-ttu-id="b98cb-109">説明</span><span class="sxs-lookup"><span data-stu-id="b98cb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b98cb-110">不明</span><span class="sxs-lookup"><span data-stu-id="b98cb-110">unknown</span></span>|<span data-ttu-id="b98cb-111">0</span><span class="sxs-lookup"><span data-stu-id="b98cb-111">0</span></span>|<span data-ttu-id="b98cb-112">不明。</span><span class="sxs-lookup"><span data-stu-id="b98cb-112">Unknown.</span></span>|
|<span data-ttu-id="b98cb-113">準拠</span><span class="sxs-lookup"><span data-stu-id="b98cb-113">compliant</span></span>|<span data-ttu-id="b98cb-114">1</span><span class="sxs-lookup"><span data-stu-id="b98cb-114">1</span></span>|<span data-ttu-id="b98cb-115">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="b98cb-115">Compliant.</span></span>|
|<span data-ttu-id="b98cb-116">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="b98cb-116">noncompliant</span></span>|<span data-ttu-id="b98cb-117">2</span><span class="sxs-lookup"><span data-stu-id="b98cb-117">2</span></span>|<span data-ttu-id="b98cb-118">デバイスは非準拠、企業のリソースがブロックされました。</span><span class="sxs-lookup"><span data-stu-id="b98cb-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="b98cb-119">競合</span><span class="sxs-lookup"><span data-stu-id="b98cb-119">conflict</span></span>|<span data-ttu-id="b98cb-120">3</span><span class="sxs-lookup"><span data-stu-id="b98cb-120">3</span></span>|<span data-ttu-id="b98cb-121">その他の規則と競合しています。</span><span class="sxs-lookup"><span data-stu-id="b98cb-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="b98cb-122">エラー</span><span class="sxs-lookup"><span data-stu-id="b98cb-122">error</span></span>|<span data-ttu-id="b98cb-123">4</span><span class="sxs-lookup"><span data-stu-id="b98cb-123">4</span></span>|<span data-ttu-id="b98cb-124">エラー。</span><span class="sxs-lookup"><span data-stu-id="b98cb-124">Error.</span></span>|
|<span data-ttu-id="b98cb-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="b98cb-125">inGracePeriod</span></span>|<span data-ttu-id="b98cb-126">254</span><span class="sxs-lookup"><span data-stu-id="b98cb-126">254</span></span>|<span data-ttu-id="b98cb-127">デバイスは非準拠ですが、社内リソースへのアクセスにはまだ</span><span class="sxs-lookup"><span data-stu-id="b98cb-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="b98cb-128">configManager</span><span class="sxs-lookup"><span data-stu-id="b98cb-128">configManager</span></span>|<span data-ttu-id="b98cb-129">255</span><span class="sxs-lookup"><span data-stu-id="b98cb-129">255</span></span>|<span data-ttu-id="b98cb-130">構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="b98cb-130">Managed by Config Manager</span></span>|



