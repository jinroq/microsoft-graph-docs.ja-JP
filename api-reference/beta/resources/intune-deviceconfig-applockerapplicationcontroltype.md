---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
ms.openlocfilehash: 150e3daa6b8deb2d1e17c3ea7caf345ba39446f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068893"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="a1d9c-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a1d9c-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="a1d9c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1d9c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1d9c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1d9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1d9c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1d9c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1d9c-107">AppLocker アプリケーションのコントロールの種類の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="a1d9c-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="a1d9c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1d9c-108">Members</span></span>
|<span data-ttu-id="a1d9c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1d9c-109">Member</span></span>|<span data-ttu-id="a1d9c-110">値</span><span class="sxs-lookup"><span data-stu-id="a1d9c-110">Value</span></span>|<span data-ttu-id="a1d9c-111">説明</span><span class="sxs-lookup"><span data-stu-id="a1d9c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1d9c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a1d9c-112">notConfigured</span></span>|<span data-ttu-id="a1d9c-113">0</span><span class="sxs-lookup"><span data-stu-id="a1d9c-113">0</span></span>|<span data-ttu-id="a1d9c-114">デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="a1d9c-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="a1d9c-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="a1d9c-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="a1d9c-116">1</span><span class="sxs-lookup"><span data-stu-id="a1d9c-116">1</span></span>|<span data-ttu-id="a1d9c-117">Windows コンポーネント、ストア アプリケーションを強制します。</span><span class="sxs-lookup"><span data-stu-id="a1d9c-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="a1d9c-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="a1d9c-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="a1d9c-119">2</span><span class="sxs-lookup"><span data-stu-id="a1d9c-119">2</span></span>|<span data-ttu-id="a1d9c-120">Windows コンポーネント、ストア アプリケーションを監査します。</span><span class="sxs-lookup"><span data-stu-id="a1d9c-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="a1d9c-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="a1d9c-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="a1d9c-122">3</span><span class="sxs-lookup"><span data-stu-id="a1d9c-122">3</span></span>|<span data-ttu-id="a1d9c-123">Windows コンポーネント、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="a1d9c-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="a1d9c-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="a1d9c-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="a1d9c-125">4</span><span class="sxs-lookup"><span data-stu-id="a1d9c-125">4</span></span>|<span data-ttu-id="a1d9c-126">Windows コンポーネントを監査し、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="a1d9c-126">Audit Windows components, store apps and smart locker.</span></span>|





