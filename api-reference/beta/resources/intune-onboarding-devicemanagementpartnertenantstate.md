---
title: deviceManagementPartnerTenantState 列挙型
description: このテナントのパートナーの状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: be116132064a562378ab664e1a22b2561e9cf20b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855504"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="fcf6e-103">deviceManagementPartnerTenantState 列挙型</span><span class="sxs-lookup"><span data-stu-id="fcf6e-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="fcf6e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcf6e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcf6e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcf6e-107">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-107">Partner state of this tenant.</span></span>
## <a name="members"></a><span data-ttu-id="fcf6e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fcf6e-108">Members</span></span>
|<span data-ttu-id="fcf6e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="fcf6e-109">Member</span></span>|<span data-ttu-id="fcf6e-110">値</span><span class="sxs-lookup"><span data-stu-id="fcf6e-110">Value</span></span>|<span data-ttu-id="fcf6e-111">説明</span><span class="sxs-lookup"><span data-stu-id="fcf6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcf6e-112">不明</span><span class="sxs-lookup"><span data-stu-id="fcf6e-112">unknown</span></span>|<span data-ttu-id="fcf6e-113">0</span><span class="sxs-lookup"><span data-stu-id="fcf6e-113">0</span></span>|<span data-ttu-id="fcf6e-114">パートナーの状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-114">Partner state is unknown.</span></span>|
|<span data-ttu-id="fcf6e-115">利用不可</span><span class="sxs-lookup"><span data-stu-id="fcf6e-115">unavailable</span></span>|<span data-ttu-id="fcf6e-116">1</span><span class="sxs-lookup"><span data-stu-id="fcf6e-116">1</span></span>|<span data-ttu-id="fcf6e-117">パートナーが利用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-117">Partner is unavailable.</span></span>|
|<span data-ttu-id="fcf6e-118">enabled</span><span class="sxs-lookup"><span data-stu-id="fcf6e-118">enabled</span></span>|<span data-ttu-id="fcf6e-119">2</span><span class="sxs-lookup"><span data-stu-id="fcf6e-119">2</span></span>|<span data-ttu-id="fcf6e-120">パートナーが有効になります。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-120">Partner is enabled.</span></span>|
|<span data-ttu-id="fcf6e-121">終了</span><span class="sxs-lookup"><span data-stu-id="fcf6e-121">terminated</span></span>|<span data-ttu-id="fcf6e-122">3</span><span class="sxs-lookup"><span data-stu-id="fcf6e-122">3</span></span>|<span data-ttu-id="fcf6e-123">パートナー接続は終了します。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-123">Partner connection is terminated.</span></span>|
|<span data-ttu-id="fcf6e-124">rejected</span><span class="sxs-lookup"><span data-stu-id="fcf6e-124">rejected</span></span>|<span data-ttu-id="fcf6e-125">4</span><span class="sxs-lookup"><span data-stu-id="fcf6e-125">4</span></span>|<span data-ttu-id="fcf6e-126">パートナーのメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-126">Partner messages are rejected.</span></span>|
|<span data-ttu-id="fcf6e-127">応答しません。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-127">unresponsive</span></span>|<span data-ttu-id="fcf6e-128">5</span><span class="sxs-lookup"><span data-stu-id="fcf6e-128">5</span></span>|<span data-ttu-id="fcf6e-129">パートナーは、応答ではありません。</span><span class="sxs-lookup"><span data-stu-id="fcf6e-129">Partner is unresponsive.</span></span>|





