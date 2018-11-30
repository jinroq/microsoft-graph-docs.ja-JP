---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
ms.openlocfilehash: 703cc18dfee49a01adb3cd4f61c5d7e99e30fb00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020752"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="3cce5-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3cce5-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="3cce5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3cce5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cce5-105">AppLocker アプリケーションのコントロールの種類の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="3cce5-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="3cce5-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="3cce5-106">Members</span></span>
|<span data-ttu-id="3cce5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3cce5-107">Member</span></span>|<span data-ttu-id="3cce5-108">値</span><span class="sxs-lookup"><span data-stu-id="3cce5-108">Value</span></span>|<span data-ttu-id="3cce5-109">説明</span><span class="sxs-lookup"><span data-stu-id="3cce5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cce5-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3cce5-110">notConfigured</span></span>|<span data-ttu-id="3cce5-111">0</span><span class="sxs-lookup"><span data-stu-id="3cce5-111">0</span></span>|<span data-ttu-id="3cce5-112">デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="3cce5-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="3cce5-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3cce5-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="3cce5-114">1</span><span class="sxs-lookup"><span data-stu-id="3cce5-114">1</span></span>|<span data-ttu-id="3cce5-115">Windows コンポーネント、ストア アプリケーションを強制します。</span><span class="sxs-lookup"><span data-stu-id="3cce5-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="3cce5-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="3cce5-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="3cce5-117">2</span><span class="sxs-lookup"><span data-stu-id="3cce5-117">2</span></span>|<span data-ttu-id="3cce5-118">Windows コンポーネント、ストア アプリケーションを監査します。</span><span class="sxs-lookup"><span data-stu-id="3cce5-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="3cce5-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3cce5-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3cce5-120">3</span><span class="sxs-lookup"><span data-stu-id="3cce5-120">3</span></span>|<span data-ttu-id="3cce5-121">Windows コンポーネント、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="3cce5-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="3cce5-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="3cce5-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="3cce5-123">4</span><span class="sxs-lookup"><span data-stu-id="3cce5-123">4</span></span>|<span data-ttu-id="3cce5-124">Windows コンポーネントを監査し、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="3cce5-124">Audit Windows components, store apps and smart locker.</span></span>|



