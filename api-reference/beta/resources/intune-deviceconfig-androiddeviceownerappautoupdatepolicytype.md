---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。
localization_priority: Normal
ms.openlocfilehash: 721d08220553bf6acfaac0f84bf0d71725c39ba6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834119"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="a5767-103">androidDeviceOwnerAppAutoUpdatePolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a5767-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="a5767-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5767-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5767-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5767-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5767-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5767-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5767-107">Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5767-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="a5767-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a5767-108">Members</span></span>
|<span data-ttu-id="a5767-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a5767-109">Member</span></span>|<span data-ttu-id="a5767-110">値</span><span class="sxs-lookup"><span data-stu-id="a5767-110">Value</span></span>|<span data-ttu-id="a5767-111">説明</span><span class="sxs-lookup"><span data-stu-id="a5767-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5767-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a5767-112">notConfigured</span></span>|<span data-ttu-id="a5767-113">0</span><span class="sxs-lookup"><span data-stu-id="a5767-113">0</span></span>|<span data-ttu-id="a5767-114">次のように構成されません。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="a5767-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="a5767-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="a5767-115">userChoice</span></span>|<span data-ttu-id="a5767-116">1</span><span class="sxs-lookup"><span data-stu-id="a5767-116">1</span></span>|<span data-ttu-id="a5767-117">ユーザーは、自動更新を制御できます。</span><span class="sxs-lookup"><span data-stu-id="a5767-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="a5767-118">ぜんぜん</span><span class="sxs-lookup"><span data-stu-id="a5767-118">never</span></span>|<span data-ttu-id="a5767-119">2</span><span class="sxs-lookup"><span data-stu-id="a5767-119">2</span></span>|<span data-ttu-id="a5767-120">アプリは自動で更新しません。</span><span class="sxs-lookup"><span data-stu-id="a5767-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="a5767-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="a5767-121">wiFiOnly</span></span>|<span data-ttu-id="a5767-122">3</span><span class="sxs-lookup"><span data-stu-id="a5767-122">3</span></span>|<span data-ttu-id="a5767-123">アプリケーションは自動的に更新 Wi-fi 経由のみです。</span><span class="sxs-lookup"><span data-stu-id="a5767-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="a5767-124">いつも</span><span class="sxs-lookup"><span data-stu-id="a5767-124">always</span></span>|<span data-ttu-id="a5767-125">4</span><span class="sxs-lookup"><span data-stu-id="a5767-125">4</span></span>|<span data-ttu-id="a5767-126">アプリケーションは、いつでも自動的に更新します。</span><span class="sxs-lookup"><span data-stu-id="a5767-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="a5767-127">データ料がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="a5767-127">Data charges may apply.</span></span>|





