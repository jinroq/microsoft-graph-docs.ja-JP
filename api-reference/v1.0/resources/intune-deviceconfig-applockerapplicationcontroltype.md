---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 241387f34a64b4b58d974fc21e2aa5d3af696736
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871982"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="9b2be-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9b2be-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="9b2be-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b2be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b2be-105">AppLocker アプリケーションのコントロールの種類の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="9b2be-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="9b2be-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="9b2be-106">Members</span></span>
|<span data-ttu-id="9b2be-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9b2be-107">Member</span></span>|<span data-ttu-id="9b2be-108">値</span><span class="sxs-lookup"><span data-stu-id="9b2be-108">Value</span></span>|<span data-ttu-id="9b2be-109">説明</span><span class="sxs-lookup"><span data-stu-id="9b2be-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b2be-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9b2be-110">notConfigured</span></span>|<span data-ttu-id="9b2be-111">0</span><span class="sxs-lookup"><span data-stu-id="9b2be-111">0</span></span>|<span data-ttu-id="9b2be-112">デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="9b2be-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="9b2be-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="9b2be-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="9b2be-114">1</span><span class="sxs-lookup"><span data-stu-id="9b2be-114">1</span></span>|<span data-ttu-id="9b2be-115">Windows コンポーネント、ストア アプリケーションを強制します。</span><span class="sxs-lookup"><span data-stu-id="9b2be-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="9b2be-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="9b2be-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="9b2be-117">2</span><span class="sxs-lookup"><span data-stu-id="9b2be-117">2</span></span>|<span data-ttu-id="9b2be-118">Windows コンポーネント、ストア アプリケーションを監査します。</span><span class="sxs-lookup"><span data-stu-id="9b2be-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="9b2be-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="9b2be-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="9b2be-120">3</span><span class="sxs-lookup"><span data-stu-id="9b2be-120">3</span></span>|<span data-ttu-id="9b2be-121">Windows コンポーネント、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="9b2be-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="9b2be-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="9b2be-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="9b2be-123">4</span><span class="sxs-lookup"><span data-stu-id="9b2be-123">4</span></span>|<span data-ttu-id="9b2be-124">Windows コンポーネントを監査し、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="9b2be-124">Audit Windows components, store apps and smart locker.</span></span>|



