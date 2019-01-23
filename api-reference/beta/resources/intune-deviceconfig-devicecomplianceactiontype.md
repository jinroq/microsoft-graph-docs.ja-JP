---
title: deviceComplianceActionType 列挙型
description: 列挙型の操作をスケジュールします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd0db68a21fff79ddbab924e8a1d9bd2ff2e542d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425744"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="bdfc9-103">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="bdfc9-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="bdfc9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bdfc9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdfc9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdfc9-107">列挙型の操作をスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-107">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="bdfc9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bdfc9-108">Members</span></span>
|<span data-ttu-id="bdfc9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="bdfc9-109">Member</span></span>|<span data-ttu-id="bdfc9-110">値</span><span class="sxs-lookup"><span data-stu-id="bdfc9-110">Value</span></span>|<span data-ttu-id="bdfc9-111">説明</span><span class="sxs-lookup"><span data-stu-id="bdfc9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdfc9-112">noAction</span><span class="sxs-lookup"><span data-stu-id="bdfc9-112">noAction</span></span>|<span data-ttu-id="bdfc9-113">0</span><span class="sxs-lookup"><span data-stu-id="bdfc9-113">0</span></span>|<span data-ttu-id="bdfc9-114">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-114">No Action</span></span>|
|<span data-ttu-id="bdfc9-115">通知</span><span class="sxs-lookup"><span data-stu-id="bdfc9-115">notification</span></span>|<span data-ttu-id="bdfc9-116">1</span><span class="sxs-lookup"><span data-stu-id="bdfc9-116">1</span></span>|<span data-ttu-id="bdfc9-117">通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-117">Send Notification</span></span>|
|<span data-ttu-id="bdfc9-118">ブロック</span><span class="sxs-lookup"><span data-stu-id="bdfc9-118">block</span></span>|<span data-ttu-id="bdfc9-119">2</span><span class="sxs-lookup"><span data-stu-id="bdfc9-119">2</span></span>|<span data-ttu-id="bdfc9-120">AAD でデバイスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-120">Block the device in AAD</span></span>|
|<span data-ttu-id="bdfc9-121">退職</span><span class="sxs-lookup"><span data-stu-id="bdfc9-121">retire</span></span>|<span data-ttu-id="bdfc9-122">3</span><span class="sxs-lookup"><span data-stu-id="bdfc9-122">3</span></span>|<span data-ttu-id="bdfc9-123">デバイスを破棄します。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-123">Retire the device</span></span>|
|<span data-ttu-id="bdfc9-124">ワイプ</span><span class="sxs-lookup"><span data-stu-id="bdfc9-124">wipe</span></span>|<span data-ttu-id="bdfc9-125">4</span><span class="sxs-lookup"><span data-stu-id="bdfc9-125">4</span></span>|<span data-ttu-id="bdfc9-126">デバイスをワイプします。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-126">Wipe the device</span></span>|
|<span data-ttu-id="bdfc9-127">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="bdfc9-127">removeResourceAccessProfiles</span></span>|<span data-ttu-id="bdfc9-128">5</span><span class="sxs-lookup"><span data-stu-id="bdfc9-128">5</span></span>|<span data-ttu-id="bdfc9-129">デバイスからリソースのアクセス ・ プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-129">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="bdfc9-130">pushNotification</span><span class="sxs-lookup"><span data-stu-id="bdfc9-130">pushNotification</span></span>|<span data-ttu-id="bdfc9-131">9</span><span class="sxs-lookup"><span data-stu-id="bdfc9-131">9</span></span>|<span data-ttu-id="bdfc9-132">デバイスにプッシュ通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-132">Send push notification to device</span></span>|
|<span data-ttu-id="bdfc9-133">remoteLock</span><span class="sxs-lookup"><span data-stu-id="bdfc9-133">remoteLock</span></span>|<span data-ttu-id="bdfc9-134">10</span><span class="sxs-lookup"><span data-stu-id="bdfc9-134">10</span></span>|<span data-ttu-id="bdfc9-135">リモートでデバイスをロックします。</span><span class="sxs-lookup"><span data-stu-id="bdfc9-135">Remotely lock the device</span></span>|




