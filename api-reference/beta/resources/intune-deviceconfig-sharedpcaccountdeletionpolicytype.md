---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 081069f9462c426f24a1e3cf276730b1db40b191
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951951"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="2fb65-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="2fb65-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="2fb65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2fb65-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fb65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fb65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fb65-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2fb65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fb65-107">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="2fb65-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="2fb65-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2fb65-108">Members</span></span>
|<span data-ttu-id="2fb65-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="2fb65-109">Member</span></span>|<span data-ttu-id="2fb65-110">値</span><span class="sxs-lookup"><span data-stu-id="2fb65-110">Value</span></span>|<span data-ttu-id="2fb65-111">説明</span><span class="sxs-lookup"><span data-stu-id="2fb65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fb65-112">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="2fb65-112">immediate</span></span>|<span data-ttu-id="2fb65-113">0</span><span class="sxs-lookup"><span data-stu-id="2fb65-113">0</span></span>|<span data-ttu-id="2fb65-114">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="2fb65-114">Delete immediately.</span></span>|
|<span data-ttu-id="2fb65-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="2fb65-115">diskSpaceThreshold</span></span>|<span data-ttu-id="2fb65-116">1</span><span class="sxs-lookup"><span data-stu-id="2fb65-116">1</span></span>|<span data-ttu-id="2fb65-117">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="2fb65-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="2fb65-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="2fb65-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="2fb65-119">2</span><span class="sxs-lookup"><span data-stu-id="2fb65-119">2</span></span>|<span data-ttu-id="2fb65-120">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="2fb65-120">Delete at disk space threshold or inactive threshold.</span></span>|





