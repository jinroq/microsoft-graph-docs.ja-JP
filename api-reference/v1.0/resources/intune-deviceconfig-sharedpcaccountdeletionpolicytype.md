---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6a1e3c9e15409e253852b4b896e18181ef1bc391
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884127"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="6a52f-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6a52f-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="6a52f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a52f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a52f-105">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="6a52f-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="6a52f-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="6a52f-106">Members</span></span>
|<span data-ttu-id="6a52f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6a52f-107">Member</span></span>|<span data-ttu-id="6a52f-108">値</span><span class="sxs-lookup"><span data-stu-id="6a52f-108">Value</span></span>|<span data-ttu-id="6a52f-109">説明</span><span class="sxs-lookup"><span data-stu-id="6a52f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a52f-110">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="6a52f-110">immediate</span></span>|<span data-ttu-id="6a52f-111">0</span><span class="sxs-lookup"><span data-stu-id="6a52f-111">0</span></span>|<span data-ttu-id="6a52f-112">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="6a52f-112">Delete immediately.</span></span>|
|<span data-ttu-id="6a52f-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="6a52f-113">diskSpaceThreshold</span></span>|<span data-ttu-id="6a52f-114">1</span><span class="sxs-lookup"><span data-stu-id="6a52f-114">1</span></span>|<span data-ttu-id="6a52f-115">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="6a52f-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="6a52f-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="6a52f-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="6a52f-117">2</span><span class="sxs-lookup"><span data-stu-id="6a52f-117">2</span></span>|<span data-ttu-id="6a52f-118">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="6a52f-118">Delete at disk space threshold or inactive threshold.</span></span>|



