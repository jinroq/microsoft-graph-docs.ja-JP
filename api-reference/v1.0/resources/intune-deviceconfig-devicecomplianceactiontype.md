---
title: deviceComplianceActionType 列挙型
description: 列挙型の操作をスケジュールします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d725213790260ece51c02bb81f2394fc8602095
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917343"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="5c099-103">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5c099-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="5c099-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c099-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c099-105">列挙型の操作をスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="5c099-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="5c099-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="5c099-106">Members</span></span>
|<span data-ttu-id="5c099-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5c099-107">Member</span></span>|<span data-ttu-id="5c099-108">値</span><span class="sxs-lookup"><span data-stu-id="5c099-108">Value</span></span>|<span data-ttu-id="5c099-109">説明</span><span class="sxs-lookup"><span data-stu-id="5c099-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c099-110">noAction</span><span class="sxs-lookup"><span data-stu-id="5c099-110">noAction</span></span>|<span data-ttu-id="5c099-111">0</span><span class="sxs-lookup"><span data-stu-id="5c099-111">0</span></span>|<span data-ttu-id="5c099-112">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="5c099-112">No Action</span></span>|
|<span data-ttu-id="5c099-113">通知</span><span class="sxs-lookup"><span data-stu-id="5c099-113">notification</span></span>|<span data-ttu-id="5c099-114">1</span><span class="sxs-lookup"><span data-stu-id="5c099-114">1</span></span>|<span data-ttu-id="5c099-115">通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="5c099-115">Send Notification</span></span>|
|<span data-ttu-id="5c099-116">ブロック</span><span class="sxs-lookup"><span data-stu-id="5c099-116">block</span></span>|<span data-ttu-id="5c099-117">2</span><span class="sxs-lookup"><span data-stu-id="5c099-117">2</span></span>|<span data-ttu-id="5c099-118">AAD でデバイスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="5c099-118">Block the device in AAD</span></span>|
|<span data-ttu-id="5c099-119">退職</span><span class="sxs-lookup"><span data-stu-id="5c099-119">retire</span></span>|<span data-ttu-id="5c099-120">3</span><span class="sxs-lookup"><span data-stu-id="5c099-120">3</span></span>|<span data-ttu-id="5c099-121">デバイスを破棄します。</span><span class="sxs-lookup"><span data-stu-id="5c099-121">Retire the device</span></span>|
|<span data-ttu-id="5c099-122">ワイプ</span><span class="sxs-lookup"><span data-stu-id="5c099-122">wipe</span></span>|<span data-ttu-id="5c099-123">4</span><span class="sxs-lookup"><span data-stu-id="5c099-123">4</span></span>|<span data-ttu-id="5c099-124">デバイスをワイプします。</span><span class="sxs-lookup"><span data-stu-id="5c099-124">Wipe the device</span></span>|
|<span data-ttu-id="5c099-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="5c099-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="5c099-126">5</span><span class="sxs-lookup"><span data-stu-id="5c099-126">5</span></span>|<span data-ttu-id="5c099-127">デバイスからリソースのアクセス ・ プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="5c099-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="5c099-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="5c099-128">pushNotification</span></span>|<span data-ttu-id="5c099-129">9</span><span class="sxs-lookup"><span data-stu-id="5c099-129">9</span></span>|<span data-ttu-id="5c099-130">デバイスにプッシュ通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="5c099-130">Send push notification to device</span></span>|



