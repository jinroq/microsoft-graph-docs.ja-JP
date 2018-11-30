---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
ms.openlocfilehash: 48d36881646bce344d99bc3d1a15a2679ddeb11d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021873"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="22dca-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="22dca-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="22dca-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="22dca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22dca-105">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="22dca-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="22dca-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="22dca-106">Members</span></span>
|<span data-ttu-id="22dca-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="22dca-107">Member</span></span>|<span data-ttu-id="22dca-108">値</span><span class="sxs-lookup"><span data-stu-id="22dca-108">Value</span></span>|<span data-ttu-id="22dca-109">説明</span><span class="sxs-lookup"><span data-stu-id="22dca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22dca-110">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="22dca-110">immediate</span></span>|<span data-ttu-id="22dca-111">0</span><span class="sxs-lookup"><span data-stu-id="22dca-111">0</span></span>|<span data-ttu-id="22dca-112">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="22dca-112">Delete immediately.</span></span>|
|<span data-ttu-id="22dca-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="22dca-113">diskSpaceThreshold</span></span>|<span data-ttu-id="22dca-114">1</span><span class="sxs-lookup"><span data-stu-id="22dca-114">1</span></span>|<span data-ttu-id="22dca-115">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="22dca-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="22dca-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="22dca-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="22dca-117">2</span><span class="sxs-lookup"><span data-stu-id="22dca-117">2</span></span>|<span data-ttu-id="22dca-118">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="22dca-118">Delete at disk space threshold or inactive threshold.</span></span>|



