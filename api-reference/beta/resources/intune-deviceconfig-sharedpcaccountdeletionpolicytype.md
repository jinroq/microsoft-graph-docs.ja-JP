---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
author: tfitzmac
ms.openlocfilehash: 626bc7ee4006639396a7959c4f09bec47c2d7f68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335050"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="9a3e8-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9a3e8-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="9a3e8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9a3e8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a3e8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a3e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a3e8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a3e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a3e8-107">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="9a3e8-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="9a3e8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9a3e8-108">Members</span></span>
|<span data-ttu-id="9a3e8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9a3e8-109">Member</span></span>|<span data-ttu-id="9a3e8-110">値</span><span class="sxs-lookup"><span data-stu-id="9a3e8-110">Value</span></span>|<span data-ttu-id="9a3e8-111">説明</span><span class="sxs-lookup"><span data-stu-id="9a3e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a3e8-112">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="9a3e8-112">immediate</span></span>|<span data-ttu-id="9a3e8-113">0</span><span class="sxs-lookup"><span data-stu-id="9a3e8-113">0</span></span>|<span data-ttu-id="9a3e8-114">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="9a3e8-114">Delete immediately.</span></span>|
|<span data-ttu-id="9a3e8-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="9a3e8-115">diskSpaceThreshold</span></span>|<span data-ttu-id="9a3e8-116">1</span><span class="sxs-lookup"><span data-stu-id="9a3e8-116">1</span></span>|<span data-ttu-id="9a3e8-117">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="9a3e8-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="9a3e8-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="9a3e8-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="9a3e8-119">2</span><span class="sxs-lookup"><span data-stu-id="9a3e8-119">2</span></span>|<span data-ttu-id="9a3e8-120">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="9a3e8-120">Delete at disk space threshold or inactive threshold.</span></span>|





