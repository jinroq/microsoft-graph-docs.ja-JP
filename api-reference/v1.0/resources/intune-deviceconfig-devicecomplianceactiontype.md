---
title: devicecomplianceactiontype 列挙型
description: スケジュールされたアクションの種類列挙
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd370f9e706955d76de519a518b4659ba46c6d25
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534312"
---
# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="42785-103">devicecomplianceactiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="42785-103">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="42785-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="42785-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42785-105">スケジュールされたアクションの種類列挙</span><span class="sxs-lookup"><span data-stu-id="42785-105">Scheduled Action Type Enum</span></span>

## <a name="members"></a><span data-ttu-id="42785-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="42785-106">Members</span></span>
|<span data-ttu-id="42785-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="42785-107">Member</span></span>|<span data-ttu-id="42785-108">値</span><span class="sxs-lookup"><span data-stu-id="42785-108">Value</span></span>|<span data-ttu-id="42785-109">説明</span><span class="sxs-lookup"><span data-stu-id="42785-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42785-110">noAction</span><span class="sxs-lookup"><span data-stu-id="42785-110">noAction</span></span>|<span data-ttu-id="42785-111">.0</span><span class="sxs-lookup"><span data-stu-id="42785-111">0</span></span>|<span data-ttu-id="42785-112">アクションなし</span><span class="sxs-lookup"><span data-stu-id="42785-112">No Action</span></span>|
|<span data-ttu-id="42785-113">お知らせ</span><span class="sxs-lookup"><span data-stu-id="42785-113">notification</span></span>|<span data-ttu-id="42785-114">1 </span><span class="sxs-lookup"><span data-stu-id="42785-114">1</span></span>|<span data-ttu-id="42785-115">通知の送信</span><span class="sxs-lookup"><span data-stu-id="42785-115">Send Notification</span></span>|
|<span data-ttu-id="42785-116">拒否</span><span class="sxs-lookup"><span data-stu-id="42785-116">block</span></span>|<span data-ttu-id="42785-117">2 </span><span class="sxs-lookup"><span data-stu-id="42785-117">2</span></span>|<span data-ttu-id="42785-118">AAD でデバイスをブロックする</span><span class="sxs-lookup"><span data-stu-id="42785-118">Block the device in AAD</span></span>|
|<span data-ttu-id="42785-119">削除</span><span class="sxs-lookup"><span data-stu-id="42785-119">retire</span></span>|<span data-ttu-id="42785-120">3 </span><span class="sxs-lookup"><span data-stu-id="42785-120">3</span></span>|<span data-ttu-id="42785-121">デバイスをインベントリから削除する</span><span class="sxs-lookup"><span data-stu-id="42785-121">Retire the device</span></span>|
|<span data-ttu-id="42785-122">ふき</span><span class="sxs-lookup"><span data-stu-id="42785-122">wipe</span></span>|<span data-ttu-id="42785-123">4 </span><span class="sxs-lookup"><span data-stu-id="42785-123">4</span></span>|<span data-ttu-id="42785-124">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="42785-124">Wipe the device</span></span>|
|<span data-ttu-id="42785-125">removeresourceaccessprofiles</span><span class="sxs-lookup"><span data-stu-id="42785-125">removeResourceAccessProfiles</span></span>|<span data-ttu-id="42785-126">5 </span><span class="sxs-lookup"><span data-stu-id="42785-126">5</span></span>|<span data-ttu-id="42785-127">デバイスからリソースアクセスプロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="42785-127">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="42785-128">pushnotification</span><span class="sxs-lookup"><span data-stu-id="42785-128">pushNotification</span></span>|<span data-ttu-id="42785-129">9 </span><span class="sxs-lookup"><span data-stu-id="42785-129">9</span></span>|<span data-ttu-id="42785-130">デバイスへのプッシュ通知の送信</span><span class="sxs-lookup"><span data-stu-id="42785-130">Send push notification to device</span></span>|



