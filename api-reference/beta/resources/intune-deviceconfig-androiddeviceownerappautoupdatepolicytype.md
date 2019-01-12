---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f784e951df2a9d1ee56825649da3899b0792c3a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973609"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="7702e-103">androidDeviceOwnerAppAutoUpdatePolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7702e-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="7702e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7702e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7702e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7702e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7702e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7702e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7702e-107">Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。</span><span class="sxs-lookup"><span data-stu-id="7702e-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="7702e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7702e-108">Members</span></span>
|<span data-ttu-id="7702e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7702e-109">Member</span></span>|<span data-ttu-id="7702e-110">値</span><span class="sxs-lookup"><span data-stu-id="7702e-110">Value</span></span>|<span data-ttu-id="7702e-111">説明</span><span class="sxs-lookup"><span data-stu-id="7702e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7702e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7702e-112">notConfigured</span></span>|<span data-ttu-id="7702e-113">0</span><span class="sxs-lookup"><span data-stu-id="7702e-113">0</span></span>|<span data-ttu-id="7702e-114">次のように構成されません。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="7702e-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="7702e-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="7702e-115">userChoice</span></span>|<span data-ttu-id="7702e-116">1</span><span class="sxs-lookup"><span data-stu-id="7702e-116">1</span></span>|<span data-ttu-id="7702e-117">ユーザーは、自動更新を制御できます。</span><span class="sxs-lookup"><span data-stu-id="7702e-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="7702e-118">ぜんぜん</span><span class="sxs-lookup"><span data-stu-id="7702e-118">never</span></span>|<span data-ttu-id="7702e-119">2</span><span class="sxs-lookup"><span data-stu-id="7702e-119">2</span></span>|<span data-ttu-id="7702e-120">アプリは自動で更新しません。</span><span class="sxs-lookup"><span data-stu-id="7702e-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="7702e-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="7702e-121">wiFiOnly</span></span>|<span data-ttu-id="7702e-122">3</span><span class="sxs-lookup"><span data-stu-id="7702e-122">3</span></span>|<span data-ttu-id="7702e-123">アプリケーションは自動的に更新 Wi-fi 経由のみです。</span><span class="sxs-lookup"><span data-stu-id="7702e-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="7702e-124">いつも</span><span class="sxs-lookup"><span data-stu-id="7702e-124">always</span></span>|<span data-ttu-id="7702e-125">4</span><span class="sxs-lookup"><span data-stu-id="7702e-125">4</span></span>|<span data-ttu-id="7702e-126">アプリケーションは、いつでも自動的に更新します。</span><span class="sxs-lookup"><span data-stu-id="7702e-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="7702e-127">データ料がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="7702e-127">Data charges may apply.</span></span>|





