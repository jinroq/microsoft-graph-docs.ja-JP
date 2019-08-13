---
title: appLockerApplicationControlType 列挙型
description: AppLocker アプリケーションコントロールタイプの可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dba073db7bf9cfb948fa5f3c76ce4294f1ee51f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333892"
---
# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="4b757-103">appLockerApplicationControlType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4b757-103">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="4b757-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b757-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b757-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b757-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b757-106">AppLocker アプリケーションコントロールタイプの可能な値</span><span class="sxs-lookup"><span data-stu-id="4b757-106">Possible values of AppLocker Application Control Types</span></span>

## <a name="members"></a><span data-ttu-id="4b757-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4b757-107">Members</span></span>
|<span data-ttu-id="4b757-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4b757-108">Member</span></span>|<span data-ttu-id="4b757-109">値</span><span class="sxs-lookup"><span data-stu-id="4b757-109">Value</span></span>|<span data-ttu-id="4b757-110">説明</span><span class="sxs-lookup"><span data-stu-id="4b757-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b757-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4b757-111">notConfigured</span></span>|<span data-ttu-id="4b757-112">.0</span><span class="sxs-lookup"><span data-stu-id="4b757-112">0</span></span>|<span data-ttu-id="4b757-113">デバイスの既定値。アプリケーションコントロールの種類は選択されていません。</span><span class="sxs-lookup"><span data-stu-id="4b757-113">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="4b757-114">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="4b757-114">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="4b757-115">1-d</span><span class="sxs-lookup"><span data-stu-id="4b757-115">1</span></span>|<span data-ttu-id="4b757-116">Windows コンポーネントおよびストアアプリを適用します。</span><span class="sxs-lookup"><span data-stu-id="4b757-116">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="4b757-117">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="4b757-117">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="4b757-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4b757-118">2</span></span>|<span data-ttu-id="4b757-119">Windows コンポーネントおよびストアアプリを監査します。</span><span class="sxs-lookup"><span data-stu-id="4b757-119">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="4b757-120">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="4b757-120">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="4b757-121">1/3</span><span class="sxs-lookup"><span data-stu-id="4b757-121">3</span></span>|<span data-ttu-id="4b757-122">Windows コンポーネント、ストアアプリ、およびスマートロッカーを適用します。</span><span class="sxs-lookup"><span data-stu-id="4b757-122">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="4b757-123">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="4b757-123">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="4b757-124">2/4</span><span class="sxs-lookup"><span data-stu-id="4b757-124">4</span></span>|<span data-ttu-id="4b757-125">Windows コンポーネント、ストアアプリ、およびスマートロッカーを監査します。</span><span class="sxs-lookup"><span data-stu-id="4b757-125">Audit Windows components, store apps and smart locker.</span></span>|



