---
title: devicecomplianceactiontype 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d824f579787bf24cc56704a1c8a9df280d969809
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173508"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="e71ad-103">devicecomplianceactiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="e71ad-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="e71ad-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e71ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e71ad-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e71ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e71ad-106">スケジュールされたアクションの種類列挙</span><span class="sxs-lookup"><span data-stu-id="e71ad-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="e71ad-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e71ad-107">Members</span></span>
|<span data-ttu-id="e71ad-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e71ad-108">Member</span></span>|<span data-ttu-id="e71ad-109">値</span><span class="sxs-lookup"><span data-stu-id="e71ad-109">Value</span></span>|<span data-ttu-id="e71ad-110">説明</span><span class="sxs-lookup"><span data-stu-id="e71ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e71ad-111">noAction</span><span class="sxs-lookup"><span data-stu-id="e71ad-111">noAction</span></span>|<span data-ttu-id="e71ad-112">.0</span><span class="sxs-lookup"><span data-stu-id="e71ad-112">0</span></span>|<span data-ttu-id="e71ad-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="e71ad-113">No Action</span></span>|
|<span data-ttu-id="e71ad-114">お知らせ</span><span class="sxs-lookup"><span data-stu-id="e71ad-114">notification</span></span>|<span data-ttu-id="e71ad-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e71ad-115">1</span></span>|<span data-ttu-id="e71ad-116">通知の送信</span><span class="sxs-lookup"><span data-stu-id="e71ad-116">Send Notification</span></span>|
|<span data-ttu-id="e71ad-117">拒否</span><span class="sxs-lookup"><span data-stu-id="e71ad-117">block</span></span>|<span data-ttu-id="e71ad-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e71ad-118">2</span></span>|<span data-ttu-id="e71ad-119">AAD でデバイスをブロックする</span><span class="sxs-lookup"><span data-stu-id="e71ad-119">Block the device in AAD</span></span>|
|<span data-ttu-id="e71ad-120">削除</span><span class="sxs-lookup"><span data-stu-id="e71ad-120">retire</span></span>|<span data-ttu-id="e71ad-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e71ad-121">3</span></span>|<span data-ttu-id="e71ad-122">デバイスをインベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="e71ad-122">Retire the device</span></span>|
|<span data-ttu-id="e71ad-123">ふき</span><span class="sxs-lookup"><span data-stu-id="e71ad-123">wipe</span></span>|<span data-ttu-id="e71ad-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e71ad-124">4</span></span>|<span data-ttu-id="e71ad-125">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="e71ad-125">Wipe the device</span></span>|
|<span data-ttu-id="e71ad-126">removeresourceaccessprofiles</span><span class="sxs-lookup"><span data-stu-id="e71ad-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="e71ad-127">5</span><span class="sxs-lookup"><span data-stu-id="e71ad-127">5</span></span>|<span data-ttu-id="e71ad-128">デバイスからリソースアクセスプロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="e71ad-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="e71ad-129">pushnotification</span><span class="sxs-lookup"><span data-stu-id="e71ad-129">pushNotification</span></span>|<span data-ttu-id="e71ad-130">i-9</span><span class="sxs-lookup"><span data-stu-id="e71ad-130">9</span></span>|<span data-ttu-id="e71ad-131">デバイスへのプッシュ通知の送信</span><span class="sxs-lookup"><span data-stu-id="e71ad-131">Send push notification to device</span></span>|
|<span data-ttu-id="e71ad-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="e71ad-132">remoteLock</span></span>|<span data-ttu-id="e71ad-133">個</span><span class="sxs-lookup"><span data-stu-id="e71ad-133">10</span></span>|<span data-ttu-id="e71ad-134">デバイスをリモートでロックする</span><span class="sxs-lookup"><span data-stu-id="e71ad-134">Remotely lock the device</span></span>|




