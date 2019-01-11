---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9ca34a44b1ea4e55199eb65283f839cb50e222da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807806"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="b7edf-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b7edf-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="b7edf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7edf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7edf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7edf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7edf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7edf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7edf-107">AppLocker アプリケーションのコントロールの種類の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="b7edf-107">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="b7edf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7edf-108">Members</span></span>
|<span data-ttu-id="b7edf-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="b7edf-109">Member</span></span>|<span data-ttu-id="b7edf-110">値</span><span class="sxs-lookup"><span data-stu-id="b7edf-110">Value</span></span>|<span data-ttu-id="b7edf-111">説明</span><span class="sxs-lookup"><span data-stu-id="b7edf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7edf-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b7edf-112">notConfigured</span></span>|<span data-ttu-id="b7edf-113">0</span><span class="sxs-lookup"><span data-stu-id="b7edf-113">0</span></span>|<span data-ttu-id="b7edf-114">デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="b7edf-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="b7edf-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="b7edf-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="b7edf-116">1</span><span class="sxs-lookup"><span data-stu-id="b7edf-116">1</span></span>|<span data-ttu-id="b7edf-117">Windows コンポーネント、ストア アプリケーションを強制します。</span><span class="sxs-lookup"><span data-stu-id="b7edf-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="b7edf-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="b7edf-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="b7edf-119">2</span><span class="sxs-lookup"><span data-stu-id="b7edf-119">2</span></span>|<span data-ttu-id="b7edf-120">Windows コンポーネント、ストア アプリケーションを監査します。</span><span class="sxs-lookup"><span data-stu-id="b7edf-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="b7edf-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="b7edf-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="b7edf-122">3</span><span class="sxs-lookup"><span data-stu-id="b7edf-122">3</span></span>|<span data-ttu-id="b7edf-123">Windows コンポーネント、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="b7edf-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="b7edf-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="b7edf-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="b7edf-125">4</span><span class="sxs-lookup"><span data-stu-id="b7edf-125">4</span></span>|<span data-ttu-id="b7edf-126">Windows コンポーネントを監査し、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="b7edf-126">Audit Windows components, store apps and smart locker.</span></span>|





