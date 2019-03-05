---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b1e463959cf4b5b39076fcf200b1c61ea0e73c0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257079"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="71be6-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="71be6-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="71be6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="71be6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71be6-105">AppLocker アプリケーションコントロールタイプの可能な値</span><span class="sxs-lookup"><span data-stu-id="71be6-105">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="71be6-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="71be6-106">Members</span></span>
|<span data-ttu-id="71be6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="71be6-107">Member</span></span>|<span data-ttu-id="71be6-108">値</span><span class="sxs-lookup"><span data-stu-id="71be6-108">Value</span></span>|<span data-ttu-id="71be6-109">説明</span><span class="sxs-lookup"><span data-stu-id="71be6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71be6-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="71be6-110">notConfigured</span></span>|<span data-ttu-id="71be6-111">.0</span><span class="sxs-lookup"><span data-stu-id="71be6-111">0</span></span>|<span data-ttu-id="71be6-112">デバイスの既定値。アプリケーションコントロールの種類は選択されていません。</span><span class="sxs-lookup"><span data-stu-id="71be6-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="71be6-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="71be6-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="71be6-114">1-d</span><span class="sxs-lookup"><span data-stu-id="71be6-114">1</span></span>|<span data-ttu-id="71be6-115">Windows コンポーネントおよびストアアプリを適用します。</span><span class="sxs-lookup"><span data-stu-id="71be6-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="71be6-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="71be6-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="71be6-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="71be6-117">2</span></span>|<span data-ttu-id="71be6-118">Windows コンポーネントおよびストアアプリを監査します。</span><span class="sxs-lookup"><span data-stu-id="71be6-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="71be6-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="71be6-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="71be6-120">1/3</span><span class="sxs-lookup"><span data-stu-id="71be6-120">3</span></span>|<span data-ttu-id="71be6-121">Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。</span><span class="sxs-lookup"><span data-stu-id="71be6-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="71be6-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="71be6-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="71be6-123">2/4</span><span class="sxs-lookup"><span data-stu-id="71be6-123">4</span></span>|<span data-ttu-id="71be6-124">Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。</span><span class="sxs-lookup"><span data-stu-id="71be6-124">Audit Windows components, store apps and smart locker.</span></span>|



