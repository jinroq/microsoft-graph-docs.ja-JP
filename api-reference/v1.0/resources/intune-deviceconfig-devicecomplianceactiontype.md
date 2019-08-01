---
title: deviceComplianceActionType 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cea72fa6e48699e540a43ea3938986e19ed351d3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028519"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="23a49-103">deviceComplianceActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="23a49-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="23a49-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23a49-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23a49-105">スケジュールされたアクションの種類列挙</span><span class="sxs-lookup"><span data-stu-id="23a49-105">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="23a49-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="23a49-106">Members</span></span>
|<span data-ttu-id="23a49-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="23a49-107">Member</span></span>|<span data-ttu-id="23a49-108">値</span><span class="sxs-lookup"><span data-stu-id="23a49-108">Value</span></span>|<span data-ttu-id="23a49-109">説明</span><span class="sxs-lookup"><span data-stu-id="23a49-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a49-110">noAction</span><span class="sxs-lookup"><span data-stu-id="23a49-110">noAction</span></span>|<span data-ttu-id="23a49-111">.0</span><span class="sxs-lookup"><span data-stu-id="23a49-111">0</span></span>|<span data-ttu-id="23a49-112">アクションなし</span><span class="sxs-lookup"><span data-stu-id="23a49-112">No Action</span></span>|
|<span data-ttu-id="23a49-113">お知らせ</span><span class="sxs-lookup"><span data-stu-id="23a49-113">notification</span></span>|<span data-ttu-id="23a49-114">1-d</span><span class="sxs-lookup"><span data-stu-id="23a49-114">1</span></span>|<span data-ttu-id="23a49-115">通知の送信</span><span class="sxs-lookup"><span data-stu-id="23a49-115">Send Notification</span></span>|
|<span data-ttu-id="23a49-116">拒否</span><span class="sxs-lookup"><span data-stu-id="23a49-116">block</span></span>|<span data-ttu-id="23a49-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="23a49-117">2</span></span>|<span data-ttu-id="23a49-118">AAD でデバイスをブロックする</span><span class="sxs-lookup"><span data-stu-id="23a49-118">Block the device in AAD</span></span>|
|<span data-ttu-id="23a49-119">削除</span><span class="sxs-lookup"><span data-stu-id="23a49-119">retire</span></span>|<span data-ttu-id="23a49-120">1/3</span><span class="sxs-lookup"><span data-stu-id="23a49-120">3</span></span>|<span data-ttu-id="23a49-121">デバイスをインベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="23a49-121">Retire the device</span></span>|
|<span data-ttu-id="23a49-122">ふき</span><span class="sxs-lookup"><span data-stu-id="23a49-122">wipe</span></span>|<span data-ttu-id="23a49-123">2/4</span><span class="sxs-lookup"><span data-stu-id="23a49-123">4</span></span>|<span data-ttu-id="23a49-124">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="23a49-124">Wipe the device</span></span>|
|<span data-ttu-id="23a49-125">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="23a49-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="23a49-126">5</span><span class="sxs-lookup"><span data-stu-id="23a49-126">5</span></span>|<span data-ttu-id="23a49-127">デバイスからリソースアクセスプロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="23a49-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="23a49-128">pushNotification</span><span class="sxs-lookup"><span data-stu-id="23a49-128">pushNotification</span></span>|<span data-ttu-id="23a49-129">9 </span><span class="sxs-lookup"><span data-stu-id="23a49-129">9</span></span>|<span data-ttu-id="23a49-130">デバイスへのプッシュ通知の送信</span><span class="sxs-lookup"><span data-stu-id="23a49-130">Send push notification to device</span></span>|



