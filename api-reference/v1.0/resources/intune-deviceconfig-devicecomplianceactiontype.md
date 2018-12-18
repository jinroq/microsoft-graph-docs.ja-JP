---
title: deviceComplianceActionType 列挙型
description: 列挙型の操作をスケジュールします。
author: tfitzmac
ms.openlocfilehash: 84bef94d7352c13b49f223b859cea218932f8cad
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328687"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="1bd7c-103">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1bd7c-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="1bd7c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bd7c-105">列挙型の操作をスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-105">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="1bd7c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1bd7c-106">Members</span></span>
|<span data-ttu-id="1bd7c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1bd7c-107">Member</span></span>|<span data-ttu-id="1bd7c-108">値</span><span class="sxs-lookup"><span data-stu-id="1bd7c-108">Value</span></span>|<span data-ttu-id="1bd7c-109">説明</span><span class="sxs-lookup"><span data-stu-id="1bd7c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bd7c-110">noAction</span><span class="sxs-lookup"><span data-stu-id="1bd7c-110">noAction</span></span>|<span data-ttu-id="1bd7c-111">0</span><span class="sxs-lookup"><span data-stu-id="1bd7c-111">0</span></span>|<span data-ttu-id="1bd7c-112">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-112">No Action</span></span>|
|<span data-ttu-id="1bd7c-113">通知</span><span class="sxs-lookup"><span data-stu-id="1bd7c-113">notification</span></span>|<span data-ttu-id="1bd7c-114">1</span><span class="sxs-lookup"><span data-stu-id="1bd7c-114">1</span></span>|<span data-ttu-id="1bd7c-115">通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-115">Send Notification</span></span>|
|<span data-ttu-id="1bd7c-116">ブロック</span><span class="sxs-lookup"><span data-stu-id="1bd7c-116">block</span></span>|<span data-ttu-id="1bd7c-117">2</span><span class="sxs-lookup"><span data-stu-id="1bd7c-117">2</span></span>|<span data-ttu-id="1bd7c-118">AAD でデバイスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-118">Block the device in AAD</span></span>|
|<span data-ttu-id="1bd7c-119">退職</span><span class="sxs-lookup"><span data-stu-id="1bd7c-119">retire</span></span>|<span data-ttu-id="1bd7c-120">3</span><span class="sxs-lookup"><span data-stu-id="1bd7c-120">3</span></span>|<span data-ttu-id="1bd7c-121">デバイスを破棄します。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-121">Retire the device</span></span>|
|<span data-ttu-id="1bd7c-122">ワイプ</span><span class="sxs-lookup"><span data-stu-id="1bd7c-122">wipe</span></span>|<span data-ttu-id="1bd7c-123">4</span><span class="sxs-lookup"><span data-stu-id="1bd7c-123">4</span></span>|<span data-ttu-id="1bd7c-124">デバイスをワイプします。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-124">Wipe the device</span></span>|
|<span data-ttu-id="1bd7c-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="1bd7c-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="1bd7c-126">5</span><span class="sxs-lookup"><span data-stu-id="1bd7c-126">5</span></span>|<span data-ttu-id="1bd7c-127">デバイスからリソースのアクセス ・ プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="1bd7c-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="1bd7c-128">pushNotification</span></span>|<span data-ttu-id="1bd7c-129">9</span><span class="sxs-lookup"><span data-stu-id="1bd7c-129">9</span></span>|<span data-ttu-id="1bd7c-130">デバイスにプッシュ通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="1bd7c-130">Send push notification to device</span></span>|



