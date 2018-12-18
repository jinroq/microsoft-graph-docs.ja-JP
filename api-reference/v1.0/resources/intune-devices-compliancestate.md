---
title: complianceState 列挙型
description: コンプライアンス状態です。
author: tfitzmac
ms.openlocfilehash: 3045685518f1c7718f9a5f46cd10e0add6fe05b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330276"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="00408-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="00408-103">complianceState enum type</span></span>

> <span data-ttu-id="00408-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="00408-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00408-105">コンプライアンス状態です。</span><span class="sxs-lookup"><span data-stu-id="00408-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="00408-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="00408-106">Members</span></span>
|<span data-ttu-id="00408-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="00408-107">Member</span></span>|<span data-ttu-id="00408-108">値</span><span class="sxs-lookup"><span data-stu-id="00408-108">Value</span></span>|<span data-ttu-id="00408-109">説明</span><span class="sxs-lookup"><span data-stu-id="00408-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00408-110">不明</span><span class="sxs-lookup"><span data-stu-id="00408-110">unknown</span></span>|<span data-ttu-id="00408-111">0</span><span class="sxs-lookup"><span data-stu-id="00408-111">0</span></span>|<span data-ttu-id="00408-112">不明。</span><span class="sxs-lookup"><span data-stu-id="00408-112">Unknown.</span></span>|
|<span data-ttu-id="00408-113">準拠</span><span class="sxs-lookup"><span data-stu-id="00408-113">compliant</span></span>|<span data-ttu-id="00408-114">1</span><span class="sxs-lookup"><span data-stu-id="00408-114">1</span></span>|<span data-ttu-id="00408-115">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="00408-115">Compliant.</span></span>|
|<span data-ttu-id="00408-116">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="00408-116">noncompliant</span></span>|<span data-ttu-id="00408-117">2</span><span class="sxs-lookup"><span data-stu-id="00408-117">2</span></span>|<span data-ttu-id="00408-118">デバイスは非準拠、企業のリソースがブロックされました。</span><span class="sxs-lookup"><span data-stu-id="00408-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="00408-119">競合</span><span class="sxs-lookup"><span data-stu-id="00408-119">conflict</span></span>|<span data-ttu-id="00408-120">3</span><span class="sxs-lookup"><span data-stu-id="00408-120">3</span></span>|<span data-ttu-id="00408-121">その他の規則と競合しています。</span><span class="sxs-lookup"><span data-stu-id="00408-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="00408-122">エラー</span><span class="sxs-lookup"><span data-stu-id="00408-122">error</span></span>|<span data-ttu-id="00408-123">4</span><span class="sxs-lookup"><span data-stu-id="00408-123">4</span></span>|<span data-ttu-id="00408-124">エラー。</span><span class="sxs-lookup"><span data-stu-id="00408-124">Error.</span></span>|
|<span data-ttu-id="00408-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="00408-125">inGracePeriod</span></span>|<span data-ttu-id="00408-126">254</span><span class="sxs-lookup"><span data-stu-id="00408-126">254</span></span>|<span data-ttu-id="00408-127">デバイスは非準拠ですが、社内リソースへのアクセスにはまだ</span><span class="sxs-lookup"><span data-stu-id="00408-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="00408-128">configManager</span><span class="sxs-lookup"><span data-stu-id="00408-128">configManager</span></span>|<span data-ttu-id="00408-129">255</span><span class="sxs-lookup"><span data-stu-id="00408-129">255</span></span>|<span data-ttu-id="00408-130">構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="00408-130">Managed by Config Manager</span></span>|



