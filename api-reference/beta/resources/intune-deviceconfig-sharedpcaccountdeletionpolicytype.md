---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d7f51f76e6164c973b213eb53526d5961bb2b627
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861034"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="b7316-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b7316-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="b7316-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7316-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7316-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7316-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7316-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7316-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7316-107">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="b7316-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="b7316-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7316-108">Members</span></span>
|<span data-ttu-id="b7316-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7316-109">Member</span></span>|<span data-ttu-id="b7316-110">値</span><span class="sxs-lookup"><span data-stu-id="b7316-110">Value</span></span>|<span data-ttu-id="b7316-111">説明</span><span class="sxs-lookup"><span data-stu-id="b7316-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7316-112">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="b7316-112">immediate</span></span>|<span data-ttu-id="b7316-113">0</span><span class="sxs-lookup"><span data-stu-id="b7316-113">0</span></span>|<span data-ttu-id="b7316-114">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="b7316-114">Delete immediately.</span></span>|
|<span data-ttu-id="b7316-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="b7316-115">diskSpaceThreshold</span></span>|<span data-ttu-id="b7316-116">1</span><span class="sxs-lookup"><span data-stu-id="b7316-116">1</span></span>|<span data-ttu-id="b7316-117">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="b7316-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="b7316-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="b7316-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="b7316-119">2</span><span class="sxs-lookup"><span data-stu-id="b7316-119">2</span></span>|<span data-ttu-id="b7316-120">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="b7316-120">Delete at disk space threshold or inactive threshold.</span></span>|





