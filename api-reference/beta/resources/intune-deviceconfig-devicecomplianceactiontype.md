---
title: devicecomplianceactiontype 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba07cb2b0fe076642cb1157a5d5df09a04a63a47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566032"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="d5425-103">devicecomplianceactiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="d5425-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="d5425-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5425-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5425-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5425-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5425-106">スケジュールされたアクションの種類列挙</span><span class="sxs-lookup"><span data-stu-id="d5425-106">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="d5425-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5425-107">Members</span></span>
|<span data-ttu-id="d5425-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5425-108">Member</span></span>|<span data-ttu-id="d5425-109">値</span><span class="sxs-lookup"><span data-stu-id="d5425-109">Value</span></span>|<span data-ttu-id="d5425-110">説明</span><span class="sxs-lookup"><span data-stu-id="d5425-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5425-111">noAction</span><span class="sxs-lookup"><span data-stu-id="d5425-111">noAction</span></span>|<span data-ttu-id="d5425-112">.0</span><span class="sxs-lookup"><span data-stu-id="d5425-112">0</span></span>|<span data-ttu-id="d5425-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="d5425-113">No Action</span></span>|
|<span data-ttu-id="d5425-114">お知らせ</span><span class="sxs-lookup"><span data-stu-id="d5425-114">notification</span></span>|<span data-ttu-id="d5425-115">1 </span><span class="sxs-lookup"><span data-stu-id="d5425-115">1</span></span>|<span data-ttu-id="d5425-116">通知の送信</span><span class="sxs-lookup"><span data-stu-id="d5425-116">Send Notification</span></span>|
|<span data-ttu-id="d5425-117">拒否</span><span class="sxs-lookup"><span data-stu-id="d5425-117">block</span></span>|<span data-ttu-id="d5425-118">2 </span><span class="sxs-lookup"><span data-stu-id="d5425-118">2</span></span>|<span data-ttu-id="d5425-119">AAD でデバイスをブロックする</span><span class="sxs-lookup"><span data-stu-id="d5425-119">Block the device in AAD</span></span>|
|<span data-ttu-id="d5425-120">削除</span><span class="sxs-lookup"><span data-stu-id="d5425-120">retire</span></span>|<span data-ttu-id="d5425-121">3 </span><span class="sxs-lookup"><span data-stu-id="d5425-121">3</span></span>|<span data-ttu-id="d5425-122">デバイスをインベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="d5425-122">Retire the device</span></span>|
|<span data-ttu-id="d5425-123">ふき</span><span class="sxs-lookup"><span data-stu-id="d5425-123">wipe</span></span>|<span data-ttu-id="d5425-124">4 </span><span class="sxs-lookup"><span data-stu-id="d5425-124">4</span></span>|<span data-ttu-id="d5425-125">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="d5425-125">Wipe the device</span></span>|
|<span data-ttu-id="d5425-126">removeresourceaccessprofiles</span><span class="sxs-lookup"><span data-stu-id="d5425-126">removeResourceAccessProfiles</span></span>|<span data-ttu-id="d5425-127">5 </span><span class="sxs-lookup"><span data-stu-id="d5425-127">5</span></span>|<span data-ttu-id="d5425-128">デバイスからリソースアクセスプロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="d5425-128">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="d5425-129">pushnotification</span><span class="sxs-lookup"><span data-stu-id="d5425-129">pushNotification</span></span>|<span data-ttu-id="d5425-130">9 </span><span class="sxs-lookup"><span data-stu-id="d5425-130">9</span></span>|<span data-ttu-id="d5425-131">デバイスへのプッシュ通知の送信</span><span class="sxs-lookup"><span data-stu-id="d5425-131">Send push notification to device</span></span>|
|<span data-ttu-id="d5425-132">remoteLock</span><span class="sxs-lookup"><span data-stu-id="d5425-132">remoteLock</span></span>|<span data-ttu-id="d5425-133">10  </span><span class="sxs-lookup"><span data-stu-id="d5425-133">10</span></span>|<span data-ttu-id="d5425-134">デバイスをリモートでロックする</span><span class="sxs-lookup"><span data-stu-id="d5425-134">Remotely lock the device</span></span>|





