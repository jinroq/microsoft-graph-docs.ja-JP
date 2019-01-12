---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5dc216d20becdc233bd1664250a958aa7208f1c2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937629"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="a2b2c-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a2b2c-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="a2b2c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2b2c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2b2c-105">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="a2b2c-105">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="a2b2c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a2b2c-106">Members</span></span>
|<span data-ttu-id="a2b2c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a2b2c-107">Member</span></span>|<span data-ttu-id="a2b2c-108">値</span><span class="sxs-lookup"><span data-stu-id="a2b2c-108">Value</span></span>|<span data-ttu-id="a2b2c-109">説明</span><span class="sxs-lookup"><span data-stu-id="a2b2c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2b2c-110">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="a2b2c-110">immediate</span></span>|<span data-ttu-id="a2b2c-111">0</span><span class="sxs-lookup"><span data-stu-id="a2b2c-111">0</span></span>|<span data-ttu-id="a2b2c-112">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="a2b2c-112">Delete immediately.</span></span>|
|<span data-ttu-id="a2b2c-113">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="a2b2c-113">diskSpaceThreshold</span></span>|<span data-ttu-id="a2b2c-114">1</span><span class="sxs-lookup"><span data-stu-id="a2b2c-114">1</span></span>|<span data-ttu-id="a2b2c-115">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="a2b2c-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="a2b2c-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="a2b2c-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="a2b2c-117">2</span><span class="sxs-lookup"><span data-stu-id="a2b2c-117">2</span></span>|<span data-ttu-id="a2b2c-118">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="a2b2c-118">Delete at disk space threshold or inactive threshold.</span></span>|



