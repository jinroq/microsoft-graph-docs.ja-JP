---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4fab692743e0e76b37e81ff88e7a4d464c96e17
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799497"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="d9459-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d9459-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="d9459-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9459-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9459-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9459-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9459-106">AppLocker アプリケーションコントロールタイプの可能な値</span><span class="sxs-lookup"><span data-stu-id="d9459-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="d9459-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9459-107">Members</span></span>
|<span data-ttu-id="d9459-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9459-108">Member</span></span>|<span data-ttu-id="d9459-109">値</span><span class="sxs-lookup"><span data-stu-id="d9459-109">Value</span></span>|<span data-ttu-id="d9459-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9459-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9459-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d9459-111">notConfigured</span></span>|<span data-ttu-id="d9459-112">.0</span><span class="sxs-lookup"><span data-stu-id="d9459-112">0</span></span>|<span data-ttu-id="d9459-113">デバイスの既定値。アプリケーションコントロールの種類は選択されていません。</span><span class="sxs-lookup"><span data-stu-id="d9459-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="d9459-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="d9459-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="d9459-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d9459-115">1</span></span>|<span data-ttu-id="d9459-116">Windows コンポーネントおよびストアアプリを適用します。</span><span class="sxs-lookup"><span data-stu-id="d9459-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="d9459-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="d9459-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="d9459-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d9459-118">2</span></span>|<span data-ttu-id="d9459-119">Windows コンポーネントおよびストアアプリを監査します。</span><span class="sxs-lookup"><span data-stu-id="d9459-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="d9459-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="d9459-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="d9459-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d9459-121">3</span></span>|<span data-ttu-id="d9459-122">Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。</span><span class="sxs-lookup"><span data-stu-id="d9459-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="d9459-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="d9459-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="d9459-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d9459-124">4</span></span>|<span data-ttu-id="d9459-125">Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。</span><span class="sxs-lookup"><span data-stu-id="d9459-125">Audit Windows components, store apps and smart locker.</span></span>|





