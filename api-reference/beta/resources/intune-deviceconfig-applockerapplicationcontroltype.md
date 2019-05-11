---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d40e76303389c95c6f68350b1c2bd1a03208d46
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947569"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="0ee0e-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0ee0e-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="0ee0e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ee0e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee0e-106">AppLocker アプリケーションコントロールタイプの可能な値</span><span class="sxs-lookup"><span data-stu-id="0ee0e-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="0ee0e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0ee0e-107">Members</span></span>
|<span data-ttu-id="0ee0e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0ee0e-108">Member</span></span>|<span data-ttu-id="0ee0e-109">値</span><span class="sxs-lookup"><span data-stu-id="0ee0e-109">Value</span></span>|<span data-ttu-id="0ee0e-110">説明</span><span class="sxs-lookup"><span data-stu-id="0ee0e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee0e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0ee0e-111">notConfigured</span></span>|<span data-ttu-id="0ee0e-112">.0</span><span class="sxs-lookup"><span data-stu-id="0ee0e-112">0</span></span>|<span data-ttu-id="0ee0e-113">デバイスの既定値。アプリケーションコントロールの種類は選択されていません。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="0ee0e-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0ee0e-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="0ee0e-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0ee0e-115">1</span></span>|<span data-ttu-id="0ee0e-116">Windows コンポーネントおよびストアアプリを適用します。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="0ee0e-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0ee0e-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="0ee0e-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0ee0e-118">2</span></span>|<span data-ttu-id="0ee0e-119">Windows コンポーネントおよびストアアプリを監査します。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="0ee0e-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0ee0e-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0ee0e-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0ee0e-121">3</span></span>|<span data-ttu-id="0ee0e-122">Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="0ee0e-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0ee0e-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0ee0e-124">2/4</span><span class="sxs-lookup"><span data-stu-id="0ee0e-124">4</span></span>|<span data-ttu-id="0ee0e-125">Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-125">Audit Windows components, store apps and smart locker.</span></span>|




