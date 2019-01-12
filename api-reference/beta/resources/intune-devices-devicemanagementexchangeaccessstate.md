---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03a407d0971059ed7a0a8bb0ffae2773bc788b31
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928396"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="17145-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="17145-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="17145-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="17145-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17145-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17145-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17145-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="17145-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17145-107">デバイスの Exchange のアクセスの状態です。</span><span class="sxs-lookup"><span data-stu-id="17145-107">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="17145-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="17145-108">Members</span></span>
|<span data-ttu-id="17145-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="17145-109">Member</span></span>|<span data-ttu-id="17145-110">値</span><span class="sxs-lookup"><span data-stu-id="17145-110">Value</span></span>|<span data-ttu-id="17145-111">説明</span><span class="sxs-lookup"><span data-stu-id="17145-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17145-112">none</span><span class="sxs-lookup"><span data-stu-id="17145-112">none</span></span>|<span data-ttu-id="17145-113">0</span><span class="sxs-lookup"><span data-stu-id="17145-113">0</span></span>|<span data-ttu-id="17145-114">Exchange から検出アクセス状態がないです。</span><span class="sxs-lookup"><span data-stu-id="17145-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="17145-115">不明</span><span class="sxs-lookup"><span data-stu-id="17145-115">unknown</span></span>|<span data-ttu-id="17145-116">1</span><span class="sxs-lookup"><span data-stu-id="17145-116">1</span></span>|<span data-ttu-id="17145-117">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="17145-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="17145-118">許可</span><span class="sxs-lookup"><span data-stu-id="17145-118">allowed</span></span>|<span data-ttu-id="17145-119">2</span><span class="sxs-lookup"><span data-stu-id="17145-119">2</span></span>|<span data-ttu-id="17145-120">デバイスが Exchange へのアクセス権を持つ</span><span class="sxs-lookup"><span data-stu-id="17145-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="17145-121">ブロック</span><span class="sxs-lookup"><span data-stu-id="17145-121">blocked</span></span>|<span data-ttu-id="17145-122">3</span><span class="sxs-lookup"><span data-stu-id="17145-122">3</span></span>|<span data-ttu-id="17145-123">デバイスが Exchange でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="17145-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="17145-124">検疫</span><span class="sxs-lookup"><span data-stu-id="17145-124">quarantined</span></span>|<span data-ttu-id="17145-125">4</span><span class="sxs-lookup"><span data-stu-id="17145-125">4</span></span>|<span data-ttu-id="17145-126">デバイスが Exchange の検疫します。</span><span class="sxs-lookup"><span data-stu-id="17145-126">Device is Quarantined in Exchange</span></span>|





