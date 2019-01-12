---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 258a98b9ec4945c807a6aae2b34a178628952ac4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937958"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="c10cf-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c10cf-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="c10cf-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c10cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c10cf-105">AppLocker アプリケーションのコントロールの種類の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="c10cf-105">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="c10cf-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="c10cf-106">Members</span></span>
|<span data-ttu-id="c10cf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c10cf-107">Member</span></span>|<span data-ttu-id="c10cf-108">値</span><span class="sxs-lookup"><span data-stu-id="c10cf-108">Value</span></span>|<span data-ttu-id="c10cf-109">説明</span><span class="sxs-lookup"><span data-stu-id="c10cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c10cf-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c10cf-110">notConfigured</span></span>|<span data-ttu-id="c10cf-111">0</span><span class="sxs-lookup"><span data-stu-id="c10cf-111">0</span></span>|<span data-ttu-id="c10cf-112">デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="c10cf-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="c10cf-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="c10cf-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="c10cf-114">1</span><span class="sxs-lookup"><span data-stu-id="c10cf-114">1</span></span>|<span data-ttu-id="c10cf-115">Windows コンポーネント、ストア アプリケーションを強制します。</span><span class="sxs-lookup"><span data-stu-id="c10cf-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="c10cf-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="c10cf-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="c10cf-117">2</span><span class="sxs-lookup"><span data-stu-id="c10cf-117">2</span></span>|<span data-ttu-id="c10cf-118">Windows コンポーネント、ストア アプリケーションを監査します。</span><span class="sxs-lookup"><span data-stu-id="c10cf-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="c10cf-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="c10cf-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c10cf-120">3</span><span class="sxs-lookup"><span data-stu-id="c10cf-120">3</span></span>|<span data-ttu-id="c10cf-121">Windows コンポーネント、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="c10cf-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="c10cf-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="c10cf-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="c10cf-123">4</span><span class="sxs-lookup"><span data-stu-id="c10cf-123">4</span></span>|<span data-ttu-id="c10cf-124">Windows コンポーネントを監査し、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="c10cf-124">Audit Windows components, store apps and smart locker.</span></span>|



