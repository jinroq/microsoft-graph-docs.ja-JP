---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセス レベルです。
author: tfitzmac
ms.openlocfilehash: 8f163c5186c1fc8dac13a22d730870c52df66a06
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320798"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="57bea-103">deviceManagementExchangeAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="57bea-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="57bea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57bea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57bea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57bea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57bea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="57bea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57bea-107">Exchange のアクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="57bea-107">Access Level in Exchange.</span></span>
## <a name="members"></a><span data-ttu-id="57bea-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="57bea-108">Members</span></span>
|<span data-ttu-id="57bea-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="57bea-109">Member</span></span>|<span data-ttu-id="57bea-110">値</span><span class="sxs-lookup"><span data-stu-id="57bea-110">Value</span></span>|<span data-ttu-id="57bea-111">説明</span><span class="sxs-lookup"><span data-stu-id="57bea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57bea-112">none</span><span class="sxs-lookup"><span data-stu-id="57bea-112">none</span></span>|<span data-ttu-id="57bea-113">0</span><span class="sxs-lookup"><span data-stu-id="57bea-113">0</span></span>|<span data-ttu-id="57bea-114">Exchange では、デバイス アクセス ルールが構成されていません。</span><span class="sxs-lookup"><span data-stu-id="57bea-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="57bea-115">許可します。</span><span class="sxs-lookup"><span data-stu-id="57bea-115">allow</span></span>|<span data-ttu-id="57bea-116">1</span><span class="sxs-lookup"><span data-stu-id="57bea-116">1</span></span>|<span data-ttu-id="57bea-117">デバイスの Exchange へのアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="57bea-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="57bea-118">ブロック</span><span class="sxs-lookup"><span data-stu-id="57bea-118">block</span></span>|<span data-ttu-id="57bea-119">2</span><span class="sxs-lookup"><span data-stu-id="57bea-119">2</span></span>|<span data-ttu-id="57bea-120">デバイスから Exchange へのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="57bea-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="57bea-121">検査</span><span class="sxs-lookup"><span data-stu-id="57bea-121">quarantine</span></span>|<span data-ttu-id="57bea-122">3</span><span class="sxs-lookup"><span data-stu-id="57bea-122">3</span></span>|<span data-ttu-id="57bea-123">デバイスを Exchange で隔離します。</span><span class="sxs-lookup"><span data-stu-id="57bea-123">Quarantine the device in Exchange.</span></span>|





