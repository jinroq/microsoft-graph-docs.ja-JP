---
title: deviceManagementPartnerTenantState 列挙型
description: このテナントのパートナーの状態です。
author: tfitzmac
ms.openlocfilehash: 84df2744a11b869492bab4f7305191cc91dc54dd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334280"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="09577-103">deviceManagementPartnerTenantState 列挙型</span><span class="sxs-lookup"><span data-stu-id="09577-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="09577-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09577-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09577-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09577-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09577-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="09577-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09577-107">このテナントのパートナーの状態です。</span><span class="sxs-lookup"><span data-stu-id="09577-107">Partner state of this tenant.</span></span>
## <a name="members"></a><span data-ttu-id="09577-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="09577-108">Members</span></span>
|<span data-ttu-id="09577-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="09577-109">Member</span></span>|<span data-ttu-id="09577-110">値</span><span class="sxs-lookup"><span data-stu-id="09577-110">Value</span></span>|<span data-ttu-id="09577-111">説明</span><span class="sxs-lookup"><span data-stu-id="09577-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09577-112">不明</span><span class="sxs-lookup"><span data-stu-id="09577-112">unknown</span></span>|<span data-ttu-id="09577-113">0</span><span class="sxs-lookup"><span data-stu-id="09577-113">0</span></span>|<span data-ttu-id="09577-114">パートナーの状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="09577-114">Partner state is unknown.</span></span>|
|<span data-ttu-id="09577-115">利用不可</span><span class="sxs-lookup"><span data-stu-id="09577-115">unavailable</span></span>|<span data-ttu-id="09577-116">1</span><span class="sxs-lookup"><span data-stu-id="09577-116">1</span></span>|<span data-ttu-id="09577-117">パートナーが利用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="09577-117">Partner is unavailable.</span></span>|
|<span data-ttu-id="09577-118">enabled</span><span class="sxs-lookup"><span data-stu-id="09577-118">enabled</span></span>|<span data-ttu-id="09577-119">2</span><span class="sxs-lookup"><span data-stu-id="09577-119">2</span></span>|<span data-ttu-id="09577-120">パートナーが有効になります。</span><span class="sxs-lookup"><span data-stu-id="09577-120">Partner is enabled.</span></span>|
|<span data-ttu-id="09577-121">終了</span><span class="sxs-lookup"><span data-stu-id="09577-121">terminated</span></span>|<span data-ttu-id="09577-122">3</span><span class="sxs-lookup"><span data-stu-id="09577-122">3</span></span>|<span data-ttu-id="09577-123">パートナー接続は終了します。</span><span class="sxs-lookup"><span data-stu-id="09577-123">Partner connection is terminated.</span></span>|
|<span data-ttu-id="09577-124">rejected</span><span class="sxs-lookup"><span data-stu-id="09577-124">rejected</span></span>|<span data-ttu-id="09577-125">4</span><span class="sxs-lookup"><span data-stu-id="09577-125">4</span></span>|<span data-ttu-id="09577-126">パートナーのメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="09577-126">Partner messages are rejected.</span></span>|
|<span data-ttu-id="09577-127">応答しません。</span><span class="sxs-lookup"><span data-stu-id="09577-127">unresponsive</span></span>|<span data-ttu-id="09577-128">5</span><span class="sxs-lookup"><span data-stu-id="09577-128">5</span></span>|<span data-ttu-id="09577-129">パートナーは、応答ではありません。</span><span class="sxs-lookup"><span data-stu-id="09577-129">Partner is unresponsive.</span></span>|





