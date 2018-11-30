---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
ms.openlocfilehash: e075f3c52dc09d2c762552d3c6580d419f0616f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069655"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="83e8a-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="83e8a-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="83e8a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83e8a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83e8a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83e8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83e8a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="83e8a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83e8a-107">デバイスの Exchange のアクセスの状態です。</span><span class="sxs-lookup"><span data-stu-id="83e8a-107">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="83e8a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="83e8a-108">Members</span></span>
|<span data-ttu-id="83e8a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="83e8a-109">Member</span></span>|<span data-ttu-id="83e8a-110">値</span><span class="sxs-lookup"><span data-stu-id="83e8a-110">Value</span></span>|<span data-ttu-id="83e8a-111">説明</span><span class="sxs-lookup"><span data-stu-id="83e8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83e8a-112">none</span><span class="sxs-lookup"><span data-stu-id="83e8a-112">none</span></span>|<span data-ttu-id="83e8a-113">0</span><span class="sxs-lookup"><span data-stu-id="83e8a-113">0</span></span>|<span data-ttu-id="83e8a-114">Exchange から検出アクセス状態がないです。</span><span class="sxs-lookup"><span data-stu-id="83e8a-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="83e8a-115">不明</span><span class="sxs-lookup"><span data-stu-id="83e8a-115">unknown</span></span>|<span data-ttu-id="83e8a-116">1</span><span class="sxs-lookup"><span data-stu-id="83e8a-116">1</span></span>|<span data-ttu-id="83e8a-117">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="83e8a-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="83e8a-118">許可</span><span class="sxs-lookup"><span data-stu-id="83e8a-118">allowed</span></span>|<span data-ttu-id="83e8a-119">2</span><span class="sxs-lookup"><span data-stu-id="83e8a-119">2</span></span>|<span data-ttu-id="83e8a-120">デバイスが Exchange へのアクセス権を持つ</span><span class="sxs-lookup"><span data-stu-id="83e8a-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="83e8a-121">ブロック</span><span class="sxs-lookup"><span data-stu-id="83e8a-121">blocked</span></span>|<span data-ttu-id="83e8a-122">3</span><span class="sxs-lookup"><span data-stu-id="83e8a-122">3</span></span>|<span data-ttu-id="83e8a-123">デバイスが Exchange でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="83e8a-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="83e8a-124">検疫</span><span class="sxs-lookup"><span data-stu-id="83e8a-124">quarantined</span></span>|<span data-ttu-id="83e8a-125">4</span><span class="sxs-lookup"><span data-stu-id="83e8a-125">4</span></span>|<span data-ttu-id="83e8a-126">デバイスが Exchange の検疫します。</span><span class="sxs-lookup"><span data-stu-id="83e8a-126">Device is Quarantined in Exchange</span></span>|





