---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange のアクセスの状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b6d831eb226648dcdbdbe470c82df900a8464a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817846"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="57cfd-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="57cfd-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="57cfd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57cfd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57cfd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57cfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57cfd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="57cfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57cfd-107">デバイスの Exchange のアクセスの状態です。</span><span class="sxs-lookup"><span data-stu-id="57cfd-107">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="57cfd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="57cfd-108">Members</span></span>
|<span data-ttu-id="57cfd-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="57cfd-109">Member</span></span>|<span data-ttu-id="57cfd-110">値</span><span class="sxs-lookup"><span data-stu-id="57cfd-110">Value</span></span>|<span data-ttu-id="57cfd-111">説明</span><span class="sxs-lookup"><span data-stu-id="57cfd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57cfd-112">none</span><span class="sxs-lookup"><span data-stu-id="57cfd-112">none</span></span>|<span data-ttu-id="57cfd-113">0</span><span class="sxs-lookup"><span data-stu-id="57cfd-113">0</span></span>|<span data-ttu-id="57cfd-114">Exchange から検出アクセス状態がないです。</span><span class="sxs-lookup"><span data-stu-id="57cfd-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="57cfd-115">不明</span><span class="sxs-lookup"><span data-stu-id="57cfd-115">unknown</span></span>|<span data-ttu-id="57cfd-116">1</span><span class="sxs-lookup"><span data-stu-id="57cfd-116">1</span></span>|<span data-ttu-id="57cfd-117">Exchange へのデバイスのアクセス状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="57cfd-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="57cfd-118">許可</span><span class="sxs-lookup"><span data-stu-id="57cfd-118">allowed</span></span>|<span data-ttu-id="57cfd-119">2</span><span class="sxs-lookup"><span data-stu-id="57cfd-119">2</span></span>|<span data-ttu-id="57cfd-120">デバイスが Exchange へのアクセス権を持つ</span><span class="sxs-lookup"><span data-stu-id="57cfd-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="57cfd-121">ブロック</span><span class="sxs-lookup"><span data-stu-id="57cfd-121">blocked</span></span>|<span data-ttu-id="57cfd-122">3</span><span class="sxs-lookup"><span data-stu-id="57cfd-122">3</span></span>|<span data-ttu-id="57cfd-123">デバイスが Exchange でブロックされています。</span><span class="sxs-lookup"><span data-stu-id="57cfd-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="57cfd-124">検疫</span><span class="sxs-lookup"><span data-stu-id="57cfd-124">quarantined</span></span>|<span data-ttu-id="57cfd-125">4</span><span class="sxs-lookup"><span data-stu-id="57cfd-125">4</span></span>|<span data-ttu-id="57cfd-126">デバイスが Exchange の検疫します。</span><span class="sxs-lookup"><span data-stu-id="57cfd-126">Device is Quarantined in Exchange</span></span>|





