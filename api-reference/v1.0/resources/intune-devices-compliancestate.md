---
title: complianceState 列挙型
description: コンプライアンス状態です。
ms.openlocfilehash: 041a2267b952d37e0aeef29e1325e5cb7b561ed7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023659"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="1493d-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="1493d-103">complianceState enum type</span></span>

> <span data-ttu-id="1493d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1493d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1493d-105">コンプライアンス状態です。</span><span class="sxs-lookup"><span data-stu-id="1493d-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="1493d-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1493d-106">Members</span></span>
|<span data-ttu-id="1493d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1493d-107">Member</span></span>|<span data-ttu-id="1493d-108">値</span><span class="sxs-lookup"><span data-stu-id="1493d-108">Value</span></span>|<span data-ttu-id="1493d-109">説明</span><span class="sxs-lookup"><span data-stu-id="1493d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1493d-110">不明</span><span class="sxs-lookup"><span data-stu-id="1493d-110">unknown</span></span>|<span data-ttu-id="1493d-111">0</span><span class="sxs-lookup"><span data-stu-id="1493d-111">0</span></span>|<span data-ttu-id="1493d-112">不明。</span><span class="sxs-lookup"><span data-stu-id="1493d-112">Unknown.</span></span>|
|<span data-ttu-id="1493d-113">準拠</span><span class="sxs-lookup"><span data-stu-id="1493d-113">compliant</span></span>|<span data-ttu-id="1493d-114">1</span><span class="sxs-lookup"><span data-stu-id="1493d-114">1</span></span>|<span data-ttu-id="1493d-115">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="1493d-115">Compliant.</span></span>|
|<span data-ttu-id="1493d-116">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="1493d-116">noncompliant</span></span>|<span data-ttu-id="1493d-117">2</span><span class="sxs-lookup"><span data-stu-id="1493d-117">2</span></span>|<span data-ttu-id="1493d-118">デバイスは非準拠、企業のリソースがブロックされました。</span><span class="sxs-lookup"><span data-stu-id="1493d-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="1493d-119">競合</span><span class="sxs-lookup"><span data-stu-id="1493d-119">conflict</span></span>|<span data-ttu-id="1493d-120">3</span><span class="sxs-lookup"><span data-stu-id="1493d-120">3</span></span>|<span data-ttu-id="1493d-121">その他の規則と競合しています。</span><span class="sxs-lookup"><span data-stu-id="1493d-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="1493d-122">エラー</span><span class="sxs-lookup"><span data-stu-id="1493d-122">error</span></span>|<span data-ttu-id="1493d-123">4</span><span class="sxs-lookup"><span data-stu-id="1493d-123">4</span></span>|<span data-ttu-id="1493d-124">エラー。</span><span class="sxs-lookup"><span data-stu-id="1493d-124">Error.</span></span>|
|<span data-ttu-id="1493d-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="1493d-125">inGracePeriod</span></span>|<span data-ttu-id="1493d-126">254</span><span class="sxs-lookup"><span data-stu-id="1493d-126">254</span></span>|<span data-ttu-id="1493d-127">デバイスは非準拠ですが、社内リソースへのアクセスにはまだ</span><span class="sxs-lookup"><span data-stu-id="1493d-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="1493d-128">configManager</span><span class="sxs-lookup"><span data-stu-id="1493d-128">configManager</span></span>|<span data-ttu-id="1493d-129">255</span><span class="sxs-lookup"><span data-stu-id="1493d-129">255</span></span>|<span data-ttu-id="1493d-130">構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="1493d-130">Managed by Config Manager</span></span>|



