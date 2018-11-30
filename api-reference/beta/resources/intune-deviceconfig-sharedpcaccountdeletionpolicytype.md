---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
ms.openlocfilehash: bf58a865dcb970760c4cf5284533cd833fcf9304
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070380"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="abed0-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="abed0-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="abed0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="abed0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abed0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abed0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abed0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="abed0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abed0-107">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="abed0-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="abed0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="abed0-108">Members</span></span>
|<span data-ttu-id="abed0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="abed0-109">Member</span></span>|<span data-ttu-id="abed0-110">値</span><span class="sxs-lookup"><span data-stu-id="abed0-110">Value</span></span>|<span data-ttu-id="abed0-111">説明</span><span class="sxs-lookup"><span data-stu-id="abed0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abed0-112">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="abed0-112">immediate</span></span>|<span data-ttu-id="abed0-113">0</span><span class="sxs-lookup"><span data-stu-id="abed0-113">0</span></span>|<span data-ttu-id="abed0-114">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="abed0-114">Delete immediately.</span></span>|
|<span data-ttu-id="abed0-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="abed0-115">diskSpaceThreshold</span></span>|<span data-ttu-id="abed0-116">1</span><span class="sxs-lookup"><span data-stu-id="abed0-116">1</span></span>|<span data-ttu-id="abed0-117">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="abed0-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="abed0-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="abed0-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="abed0-119">2</span><span class="sxs-lookup"><span data-stu-id="abed0-119">2</span></span>|<span data-ttu-id="abed0-120">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="abed0-120">Delete at disk space threshold or inactive threshold.</span></span>|





