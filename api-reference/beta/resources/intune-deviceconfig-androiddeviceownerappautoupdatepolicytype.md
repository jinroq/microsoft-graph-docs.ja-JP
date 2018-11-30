---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。
ms.openlocfilehash: 0287a26b4974bc0b376341ca91791d1fa768a9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066483"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="f90e7-103">androidDeviceOwnerAppAutoUpdatePolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f90e7-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="f90e7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f90e7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f90e7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f90e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f90e7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f90e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f90e7-107">Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。</span><span class="sxs-lookup"><span data-stu-id="f90e7-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>
## <a name="members"></a><span data-ttu-id="f90e7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f90e7-108">Members</span></span>
|<span data-ttu-id="f90e7-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f90e7-109">Member</span></span>|<span data-ttu-id="f90e7-110">値</span><span class="sxs-lookup"><span data-stu-id="f90e7-110">Value</span></span>|<span data-ttu-id="f90e7-111">説明</span><span class="sxs-lookup"><span data-stu-id="f90e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f90e7-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f90e7-112">notConfigured</span></span>|<span data-ttu-id="f90e7-113">0</span><span class="sxs-lookup"><span data-stu-id="f90e7-113">0</span></span>|<span data-ttu-id="f90e7-114">次のように構成されません。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="f90e7-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="f90e7-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="f90e7-115">userChoice</span></span>|<span data-ttu-id="f90e7-116">1</span><span class="sxs-lookup"><span data-stu-id="f90e7-116">1</span></span>|<span data-ttu-id="f90e7-117">ユーザーは、自動更新を制御できます。</span><span class="sxs-lookup"><span data-stu-id="f90e7-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="f90e7-118">ぜんぜん</span><span class="sxs-lookup"><span data-stu-id="f90e7-118">never</span></span>|<span data-ttu-id="f90e7-119">2</span><span class="sxs-lookup"><span data-stu-id="f90e7-119">2</span></span>|<span data-ttu-id="f90e7-120">アプリは自動で更新しません。</span><span class="sxs-lookup"><span data-stu-id="f90e7-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="f90e7-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="f90e7-121">wiFiOnly</span></span>|<span data-ttu-id="f90e7-122">3</span><span class="sxs-lookup"><span data-stu-id="f90e7-122">3</span></span>|<span data-ttu-id="f90e7-123">アプリケーションは自動的に更新 Wi-fi 経由のみです。</span><span class="sxs-lookup"><span data-stu-id="f90e7-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="f90e7-124">いつも</span><span class="sxs-lookup"><span data-stu-id="f90e7-124">always</span></span>|<span data-ttu-id="f90e7-125">4</span><span class="sxs-lookup"><span data-stu-id="f90e7-125">4</span></span>|<span data-ttu-id="f90e7-126">アプリケーションは、いつでも自動的に更新します。</span><span class="sxs-lookup"><span data-stu-id="f90e7-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="f90e7-127">データ料がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f90e7-127">Data charges may apply.</span></span>|





