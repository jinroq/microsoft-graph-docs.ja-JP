---
title: deviceComplianceActionType 列挙型
description: 列挙型の操作をスケジュールします。
ms.openlocfilehash: e0ec7380dcf581d811057ff5bf87edbc376d70c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020206"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="91a6d-103">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="91a6d-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="91a6d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="91a6d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91a6d-105">列挙型の操作をスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="91a6d-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="91a6d-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="91a6d-106">Members</span></span>
|<span data-ttu-id="91a6d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="91a6d-107">Member</span></span>|<span data-ttu-id="91a6d-108">値</span><span class="sxs-lookup"><span data-stu-id="91a6d-108">Value</span></span>|<span data-ttu-id="91a6d-109">説明</span><span class="sxs-lookup"><span data-stu-id="91a6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91a6d-110">noAction</span><span class="sxs-lookup"><span data-stu-id="91a6d-110">noAction</span></span>|<span data-ttu-id="91a6d-111">0</span><span class="sxs-lookup"><span data-stu-id="91a6d-111">0</span></span>|<span data-ttu-id="91a6d-112">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="91a6d-112">No Action</span></span>|
|<span data-ttu-id="91a6d-113">通知</span><span class="sxs-lookup"><span data-stu-id="91a6d-113">notification</span></span>|<span data-ttu-id="91a6d-114">1</span><span class="sxs-lookup"><span data-stu-id="91a6d-114">1</span></span>|<span data-ttu-id="91a6d-115">通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="91a6d-115">Send Notification</span></span>|
|<span data-ttu-id="91a6d-116">ブロック</span><span class="sxs-lookup"><span data-stu-id="91a6d-116">block</span></span>|<span data-ttu-id="91a6d-117">2</span><span class="sxs-lookup"><span data-stu-id="91a6d-117">2</span></span>|<span data-ttu-id="91a6d-118">AAD でデバイスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="91a6d-118">Block the device in AAD</span></span>|
|<span data-ttu-id="91a6d-119">退職</span><span class="sxs-lookup"><span data-stu-id="91a6d-119">retire</span></span>|<span data-ttu-id="91a6d-120">3</span><span class="sxs-lookup"><span data-stu-id="91a6d-120">3</span></span>|<span data-ttu-id="91a6d-121">デバイスを破棄します。</span><span class="sxs-lookup"><span data-stu-id="91a6d-121">Retire the device</span></span>|
|<span data-ttu-id="91a6d-122">ワイプ</span><span class="sxs-lookup"><span data-stu-id="91a6d-122">wipe</span></span>|<span data-ttu-id="91a6d-123">4</span><span class="sxs-lookup"><span data-stu-id="91a6d-123">4</span></span>|<span data-ttu-id="91a6d-124">デバイスをワイプします。</span><span class="sxs-lookup"><span data-stu-id="91a6d-124">Wipe the device</span></span>|
|<span data-ttu-id="91a6d-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="91a6d-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="91a6d-126">5</span><span class="sxs-lookup"><span data-stu-id="91a6d-126">5</span></span>|<span data-ttu-id="91a6d-127">デバイスからリソースのアクセス ・ プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="91a6d-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="91a6d-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="91a6d-128">pushNotification</span></span>|<span data-ttu-id="91a6d-129">9</span><span class="sxs-lookup"><span data-stu-id="91a6d-129">9</span></span>|<span data-ttu-id="91a6d-130">デバイスにプッシュ通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="91a6d-130">Send push notification to device</span></span>|



