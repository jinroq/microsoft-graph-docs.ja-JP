---
title: devicecomplianceactiontype 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd370f9e706955d76de519a518b4659ba46c6d25
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250916"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="efe0b-103">devicecomplianceactiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="efe0b-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="efe0b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="efe0b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efe0b-105">スケジュールされたアクションの種類列挙</span><span class="sxs-lookup"><span data-stu-id="efe0b-105">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="efe0b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="efe0b-106">Members</span></span>
|<span data-ttu-id="efe0b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="efe0b-107">Member</span></span>|<span data-ttu-id="efe0b-108">値</span><span class="sxs-lookup"><span data-stu-id="efe0b-108">Value</span></span>|<span data-ttu-id="efe0b-109">説明</span><span class="sxs-lookup"><span data-stu-id="efe0b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efe0b-110">noAction</span><span class="sxs-lookup"><span data-stu-id="efe0b-110">noAction</span></span>|<span data-ttu-id="efe0b-111">.0</span><span class="sxs-lookup"><span data-stu-id="efe0b-111">0</span></span>|<span data-ttu-id="efe0b-112">アクションなし</span><span class="sxs-lookup"><span data-stu-id="efe0b-112">No Action</span></span>|
|<span data-ttu-id="efe0b-113">お知らせ</span><span class="sxs-lookup"><span data-stu-id="efe0b-113">notification</span></span>|<span data-ttu-id="efe0b-114">1-d</span><span class="sxs-lookup"><span data-stu-id="efe0b-114">1</span></span>|<span data-ttu-id="efe0b-115">通知の送信</span><span class="sxs-lookup"><span data-stu-id="efe0b-115">Send Notification</span></span>|
|<span data-ttu-id="efe0b-116">拒否</span><span class="sxs-lookup"><span data-stu-id="efe0b-116">block</span></span>|<span data-ttu-id="efe0b-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="efe0b-117">2</span></span>|<span data-ttu-id="efe0b-118">AAD でデバイスをブロックする</span><span class="sxs-lookup"><span data-stu-id="efe0b-118">Block the device in AAD</span></span>|
|<span data-ttu-id="efe0b-119">削除</span><span class="sxs-lookup"><span data-stu-id="efe0b-119">retire</span></span>|<span data-ttu-id="efe0b-120">1/3</span><span class="sxs-lookup"><span data-stu-id="efe0b-120">3</span></span>|<span data-ttu-id="efe0b-121">デバイスをインベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="efe0b-121">Retire the device</span></span>|
|<span data-ttu-id="efe0b-122">ふき</span><span class="sxs-lookup"><span data-stu-id="efe0b-122">wipe</span></span>|<span data-ttu-id="efe0b-123">2/4</span><span class="sxs-lookup"><span data-stu-id="efe0b-123">4</span></span>|<span data-ttu-id="efe0b-124">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="efe0b-124">Wipe the device</span></span>|
|<span data-ttu-id="efe0b-125">removeresourceaccessprofiles</span><span class="sxs-lookup"><span data-stu-id="efe0b-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="efe0b-126">5</span><span class="sxs-lookup"><span data-stu-id="efe0b-126">5</span></span>|<span data-ttu-id="efe0b-127">デバイスからリソースアクセスプロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="efe0b-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="efe0b-128">pushnotification</span><span class="sxs-lookup"><span data-stu-id="efe0b-128">pushNotification</span></span>|<span data-ttu-id="efe0b-129">i-9</span><span class="sxs-lookup"><span data-stu-id="efe0b-129">9</span></span>|<span data-ttu-id="efe0b-130">デバイスへのプッシュ通知の送信</span><span class="sxs-lookup"><span data-stu-id="efe0b-130">Send push notification to device</span></span>|



