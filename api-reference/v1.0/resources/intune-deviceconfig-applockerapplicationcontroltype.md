---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9b4a20a79454f1aba1f162812a7fc4d7a324c359
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028568"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="9e79d-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9e79d-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="9e79d-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e79d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e79d-105">AppLocker アプリケーションコントロールタイプの可能な値</span><span class="sxs-lookup"><span data-stu-id="9e79d-105">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="9e79d-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e79d-106">Members</span></span>
|<span data-ttu-id="9e79d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9e79d-107">Member</span></span>|<span data-ttu-id="9e79d-108">値</span><span class="sxs-lookup"><span data-stu-id="9e79d-108">Value</span></span>|<span data-ttu-id="9e79d-109">説明</span><span class="sxs-lookup"><span data-stu-id="9e79d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e79d-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9e79d-110">notConfigured</span></span>|<span data-ttu-id="9e79d-111">.0</span><span class="sxs-lookup"><span data-stu-id="9e79d-111">0</span></span>|<span data-ttu-id="9e79d-112">デバイスの既定値。アプリケーションコントロールの種類は選択されていません。</span><span class="sxs-lookup"><span data-stu-id="9e79d-112">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="9e79d-113">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="9e79d-113">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="9e79d-114">1-d</span><span class="sxs-lookup"><span data-stu-id="9e79d-114">1</span></span>|<span data-ttu-id="9e79d-115">Windows コンポーネントおよびストアアプリを適用します。</span><span class="sxs-lookup"><span data-stu-id="9e79d-115">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="9e79d-116">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="9e79d-116">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="9e79d-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9e79d-117">2</span></span>|<span data-ttu-id="9e79d-118">Windows コンポーネントおよびストアアプリを監査します。</span><span class="sxs-lookup"><span data-stu-id="9e79d-118">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="9e79d-119">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="9e79d-119">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="9e79d-120">1/3</span><span class="sxs-lookup"><span data-stu-id="9e79d-120">3</span></span>|<span data-ttu-id="9e79d-121">Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。</span><span class="sxs-lookup"><span data-stu-id="9e79d-121">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="9e79d-122">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="9e79d-122">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="9e79d-123">2/4</span><span class="sxs-lookup"><span data-stu-id="9e79d-123">4</span></span>|<span data-ttu-id="9e79d-124">Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。</span><span class="sxs-lookup"><span data-stu-id="9e79d-124">Audit Windows components, store apps and smart locker.</span></span>|



