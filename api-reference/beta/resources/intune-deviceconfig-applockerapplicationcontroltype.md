---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1b3e5ec545f4466eb080f20839e12c7e5972cc0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981581"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="0d63f-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0d63f-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="0d63f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d63f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d63f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d63f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d63f-106">AppLocker アプリケーションコントロールタイプの可能な値</span><span class="sxs-lookup"><span data-stu-id="0d63f-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="0d63f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0d63f-107">Members</span></span>
|<span data-ttu-id="0d63f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0d63f-108">Member</span></span>|<span data-ttu-id="0d63f-109">値</span><span class="sxs-lookup"><span data-stu-id="0d63f-109">Value</span></span>|<span data-ttu-id="0d63f-110">説明</span><span class="sxs-lookup"><span data-stu-id="0d63f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d63f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0d63f-111">notConfigured</span></span>|<span data-ttu-id="0d63f-112">.0</span><span class="sxs-lookup"><span data-stu-id="0d63f-112">0</span></span>|<span data-ttu-id="0d63f-113">デバイスの既定値。アプリケーションコントロールの種類は選択されていません。</span><span class="sxs-lookup"><span data-stu-id="0d63f-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="0d63f-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0d63f-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="0d63f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0d63f-115">1</span></span>|<span data-ttu-id="0d63f-116">Windows コンポーネントおよびストアアプリを適用します。</span><span class="sxs-lookup"><span data-stu-id="0d63f-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="0d63f-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="0d63f-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="0d63f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0d63f-118">2</span></span>|<span data-ttu-id="0d63f-119">Windows コンポーネントおよびストアアプリを監査します。</span><span class="sxs-lookup"><span data-stu-id="0d63f-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="0d63f-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0d63f-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0d63f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0d63f-121">3</span></span>|<span data-ttu-id="0d63f-122">Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。</span><span class="sxs-lookup"><span data-stu-id="0d63f-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="0d63f-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="0d63f-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="0d63f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="0d63f-124">4</span></span>|<span data-ttu-id="0d63f-125">Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。</span><span class="sxs-lookup"><span data-stu-id="0d63f-125">Audit Windows components, store apps and smart locker.</span></span>|





