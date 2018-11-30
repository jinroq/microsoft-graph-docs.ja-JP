---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
ms.openlocfilehash: e4891656a85f91c520c783d9e5ce6beac8b08253
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021379"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="13ebd-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="13ebd-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="13ebd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="13ebd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13ebd-105">デバイスの Exchange のアクセスの状態です。</span><span class="sxs-lookup"><span data-stu-id="13ebd-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="13ebd-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="13ebd-106">Members</span></span>
|<span data-ttu-id="13ebd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="13ebd-107">Member</span></span>|<span data-ttu-id="13ebd-108">値</span><span class="sxs-lookup"><span data-stu-id="13ebd-108">Value</span></span>|<span data-ttu-id="13ebd-109">説明</span><span class="sxs-lookup"><span data-stu-id="13ebd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ebd-110">none</span><span class="sxs-lookup"><span data-stu-id="13ebd-110">none</span></span>|<span data-ttu-id="13ebd-111">0</span><span class="sxs-lookup"><span data-stu-id="13ebd-111">0</span></span>|<span data-ttu-id="13ebd-112">Exchange から検出アクセス状態がないです。</span><span class="sxs-lookup"><span data-stu-id="13ebd-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="13ebd-113">不明</span><span class="sxs-lookup"><span data-stu-id="13ebd-113">unknown</span></span>|<span data-ttu-id="13ebd-114">1</span><span class="sxs-lookup"><span data-stu-id="13ebd-114">1</span></span>|<span data-ttu-id="13ebd-115">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="13ebd-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="13ebd-116">許可</span><span class="sxs-lookup"><span data-stu-id="13ebd-116">allowed</span></span>|<span data-ttu-id="13ebd-117">2</span><span class="sxs-lookup"><span data-stu-id="13ebd-117">2</span></span>|<span data-ttu-id="13ebd-118">デバイスが Exchange へのアクセス権を持つ</span><span class="sxs-lookup"><span data-stu-id="13ebd-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="13ebd-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="13ebd-119">blocked</span></span>|<span data-ttu-id="13ebd-120">3</span><span class="sxs-lookup"><span data-stu-id="13ebd-120">3</span></span>|<span data-ttu-id="13ebd-121">デバイスが Exchange でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="13ebd-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="13ebd-122">検疫</span><span class="sxs-lookup"><span data-stu-id="13ebd-122">quarantined</span></span>|<span data-ttu-id="13ebd-123">4</span><span class="sxs-lookup"><span data-stu-id="13ebd-123">4</span></span>|<span data-ttu-id="13ebd-124">デバイスが Exchange の検疫します。</span><span class="sxs-lookup"><span data-stu-id="13ebd-124">Device is Quarantined in Exchange</span></span>|



