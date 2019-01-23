---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションのコントロールの種類の使用可能な値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3bc89620a6dd13a65cfe40f37ba2f775e6a9c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425723"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="6d5e5-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6d5e5-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="6d5e5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6d5e5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6d5e5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d5e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d5e5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d5e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d5e5-107">AppLocker アプリケーションのコントロールの種類の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="6d5e5-107">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="6d5e5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6d5e5-108">Members</span></span>
|<span data-ttu-id="6d5e5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6d5e5-109">Member</span></span>|<span data-ttu-id="6d5e5-110">値</span><span class="sxs-lookup"><span data-stu-id="6d5e5-110">Value</span></span>|<span data-ttu-id="6d5e5-111">説明</span><span class="sxs-lookup"><span data-stu-id="6d5e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d5e5-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6d5e5-112">notConfigured</span></span>|<span data-ttu-id="6d5e5-113">0</span><span class="sxs-lookup"><span data-stu-id="6d5e5-113">0</span></span>|<span data-ttu-id="6d5e5-114">デバイス デフォルト値が選択されていないアプリケーションのコントロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="6d5e5-114">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="6d5e5-115">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="6d5e5-115">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="6d5e5-116">1</span><span class="sxs-lookup"><span data-stu-id="6d5e5-116">1</span></span>|<span data-ttu-id="6d5e5-117">Windows コンポーネント、ストア アプリケーションを強制します。</span><span class="sxs-lookup"><span data-stu-id="6d5e5-117">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="6d5e5-118">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="6d5e5-118">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="6d5e5-119">2</span><span class="sxs-lookup"><span data-stu-id="6d5e5-119">2</span></span>|<span data-ttu-id="6d5e5-120">Windows コンポーネント、ストア アプリケーションを監査します。</span><span class="sxs-lookup"><span data-stu-id="6d5e5-120">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="6d5e5-121">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="6d5e5-121">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="6d5e5-122">3</span><span class="sxs-lookup"><span data-stu-id="6d5e5-122">3</span></span>|<span data-ttu-id="6d5e5-123">Windows コンポーネント、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="6d5e5-123">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="6d5e5-124">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="6d5e5-124">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="6d5e5-125">4</span><span class="sxs-lookup"><span data-stu-id="6d5e5-125">4</span></span>|<span data-ttu-id="6d5e5-126">Windows コンポーネントを監査し、アプリケーションとスマート ロッカーを格納します。</span><span class="sxs-lookup"><span data-stu-id="6d5e5-126">Audit Windows components, store apps and smart locker.</span></span>|




