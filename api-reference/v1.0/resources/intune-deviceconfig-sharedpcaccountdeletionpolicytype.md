---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
author: tfitzmac
ms.openlocfilehash: 8789faeeec7772cd6115cae82691c62894446f59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301002"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="507b7-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="507b7-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="507b7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="507b7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="507b7-105">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="507b7-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="507b7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="507b7-106">Members</span></span>
|<span data-ttu-id="507b7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="507b7-107">Member</span></span>|<span data-ttu-id="507b7-108">値</span><span class="sxs-lookup"><span data-stu-id="507b7-108">Value</span></span>|<span data-ttu-id="507b7-109">説明</span><span class="sxs-lookup"><span data-stu-id="507b7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="507b7-110">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="507b7-110">immediate</span></span>|<span data-ttu-id="507b7-111">0</span><span class="sxs-lookup"><span data-stu-id="507b7-111">0</span></span>|<span data-ttu-id="507b7-112">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="507b7-112">Delete immediately.</span></span>|
|<span data-ttu-id="507b7-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="507b7-113">diskSpaceThreshold</span></span>|<span data-ttu-id="507b7-114">1</span><span class="sxs-lookup"><span data-stu-id="507b7-114">1</span></span>|<span data-ttu-id="507b7-115">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="507b7-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="507b7-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="507b7-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="507b7-117">2</span><span class="sxs-lookup"><span data-stu-id="507b7-117">2</span></span>|<span data-ttu-id="507b7-118">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="507b7-118">Delete at disk space threshold or inactive threshold.</span></span>|



