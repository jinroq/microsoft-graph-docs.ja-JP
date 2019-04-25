---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b1e463959cf4b5b39076fcf200b1c61ea0e73c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575129"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="0f470-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0f470-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="0f470-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f470-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f470-105">AppLocker アプリケーションコントロールタイプの可能な値</span><span class="sxs-lookup"><span data-stu-id="0f470-105">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="0f470-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0f470-106">Members</span></span>
|<span data-ttu-id="0f470-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0f470-107">Member</span></span>|<span data-ttu-id="0f470-108">値</span><span class="sxs-lookup"><span data-stu-id="0f470-108">Value</span></span>|<span data-ttu-id="0f470-109">説明</span><span class="sxs-lookup"><span data-stu-id="0f470-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f470-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0f470-110">notConfigured</span></span>|<span data-ttu-id="0f470-111">.0</span><span class="sxs-lookup"><span data-stu-id="0f470-111">0</span></span>|<span data-ttu-id="0f470-112">デバイスの既定値。アプリケーションコントロールの種類は選択されていません。</span><span class="sxs-lookup"><span data-stu-id="0f470-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="0f470-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0f470-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="0f470-114">1 </span><span class="sxs-lookup"><span data-stu-id="0f470-114">1</span></span>|<span data-ttu-id="0f470-115">Windows コンポーネントおよびストアアプリを適用します。</span><span class="sxs-lookup"><span data-stu-id="0f470-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="0f470-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0f470-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="0f470-117">2 </span><span class="sxs-lookup"><span data-stu-id="0f470-117">2</span></span>|<span data-ttu-id="0f470-118">Windows コンポーネントおよびストアアプリを監査します。</span><span class="sxs-lookup"><span data-stu-id="0f470-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="0f470-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0f470-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0f470-120">3 </span><span class="sxs-lookup"><span data-stu-id="0f470-120">3</span></span>|<span data-ttu-id="0f470-121">Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。</span><span class="sxs-lookup"><span data-stu-id="0f470-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="0f470-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0f470-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0f470-123">4 </span><span class="sxs-lookup"><span data-stu-id="0f470-123">4</span></span>|<span data-ttu-id="0f470-124">Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。</span><span class="sxs-lookup"><span data-stu-id="0f470-124">Audit Windows components, store apps and smart locker.</span></span>|



