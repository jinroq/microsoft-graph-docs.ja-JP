---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dbfa7b9396a1100f2e3c7e4e78cf697233d840cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947016"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="2e728-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="2e728-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="2e728-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e728-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e728-105">デバイスの Exchange のアクセスの状態です。</span><span class="sxs-lookup"><span data-stu-id="2e728-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="2e728-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="2e728-106">Members</span></span>
|<span data-ttu-id="2e728-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2e728-107">Member</span></span>|<span data-ttu-id="2e728-108">値</span><span class="sxs-lookup"><span data-stu-id="2e728-108">Value</span></span>|<span data-ttu-id="2e728-109">説明</span><span class="sxs-lookup"><span data-stu-id="2e728-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e728-110">none</span><span class="sxs-lookup"><span data-stu-id="2e728-110">none</span></span>|<span data-ttu-id="2e728-111">0</span><span class="sxs-lookup"><span data-stu-id="2e728-111">0</span></span>|<span data-ttu-id="2e728-112">Exchange から検出アクセス状態がないです。</span><span class="sxs-lookup"><span data-stu-id="2e728-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="2e728-113">不明</span><span class="sxs-lookup"><span data-stu-id="2e728-113">unknown</span></span>|<span data-ttu-id="2e728-114">1</span><span class="sxs-lookup"><span data-stu-id="2e728-114">1</span></span>|<span data-ttu-id="2e728-115">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="2e728-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="2e728-116">許可</span><span class="sxs-lookup"><span data-stu-id="2e728-116">allowed</span></span>|<span data-ttu-id="2e728-117">2</span><span class="sxs-lookup"><span data-stu-id="2e728-117">2</span></span>|<span data-ttu-id="2e728-118">デバイスが Exchange へのアクセス権を持つ</span><span class="sxs-lookup"><span data-stu-id="2e728-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="2e728-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="2e728-119">blocked</span></span>|<span data-ttu-id="2e728-120">3</span><span class="sxs-lookup"><span data-stu-id="2e728-120">3</span></span>|<span data-ttu-id="2e728-121">デバイスが Exchange でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="2e728-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="2e728-122">検疫</span><span class="sxs-lookup"><span data-stu-id="2e728-122">quarantined</span></span>|<span data-ttu-id="2e728-123">4</span><span class="sxs-lookup"><span data-stu-id="2e728-123">4</span></span>|<span data-ttu-id="2e728-124">デバイスが Exchange の検疫します。</span><span class="sxs-lookup"><span data-stu-id="2e728-124">Device is Quarantined in Exchange</span></span>|



