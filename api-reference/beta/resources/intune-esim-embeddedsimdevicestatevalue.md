---
title: embeddedSIMDeviceStateValue 列挙型
description: SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3974c0df65ef9f59242f390b7166e11c3e0c592
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886059"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="ec072-103">embeddedSIMDeviceStateValue 列挙型</span><span class="sxs-lookup"><span data-stu-id="ec072-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="ec072-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ec072-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec072-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec072-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec072-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec072-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec072-107">SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ec072-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="ec072-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec072-108">Members</span></span>
|<span data-ttu-id="ec072-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec072-109">Member</span></span>|<span data-ttu-id="ec072-110">値</span><span class="sxs-lookup"><span data-stu-id="ec072-110">Value</span></span>|<span data-ttu-id="ec072-111">説明</span><span class="sxs-lookup"><span data-stu-id="ec072-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec072-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="ec072-112">notEvaluated</span></span>|<span data-ttu-id="ec072-113">0</span><span class="sxs-lookup"><span data-stu-id="ec072-113">0</span></span>|<span data-ttu-id="ec072-114">SIM の埋め込みのライセンス認証コードが空き時間と、デバイスに割り当てられる利用可能なことを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec072-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="ec072-115">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="ec072-115">failed</span></span>|<span data-ttu-id="ec072-116">1</span><span class="sxs-lookup"><span data-stu-id="ec072-116">1</span></span>|<span data-ttu-id="ec072-117">Intune サービスがデバイスにこのプロファイルを提供する失敗したことを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec072-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="ec072-118">インストール</span><span class="sxs-lookup"><span data-stu-id="ec072-118">installing</span></span>|<span data-ttu-id="ec072-119">2</span><span class="sxs-lookup"><span data-stu-id="ec072-119">2</span></span>|<span data-ttu-id="ec072-120">SIM の埋め込みのライセンス認証コードは、デバイスに割り当てられているし、デバイスが、トークンをインストールすることを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec072-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="ec072-121">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="ec072-121">installed</span></span>|<span data-ttu-id="ec072-122">3</span><span class="sxs-lookup"><span data-stu-id="ec072-122">3</span></span>|<span data-ttu-id="ec072-123">SIM の埋め込みのライセンス認証コードがターゲット ・ デバイスを正常にインストールされているかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec072-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="ec072-124">削除</span><span class="sxs-lookup"><span data-stu-id="ec072-124">deleting</span></span>|<span data-ttu-id="ec072-125">4</span><span class="sxs-lookup"><span data-stu-id="ec072-125">4</span></span>|<span data-ttu-id="ec072-126">Intune サービスがデバイスのプロファイルを削除しようとしていることを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec072-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="ec072-127">エラー</span><span class="sxs-lookup"><span data-stu-id="ec072-127">error</span></span>|<span data-ttu-id="ec072-128">5</span><span class="sxs-lookup"><span data-stu-id="ec072-128">5</span></span>|<span data-ttu-id="ec072-129">このプロファイルを使用してエラーがあることを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec072-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="ec072-130">deleted</span><span class="sxs-lookup"><span data-stu-id="ec072-130">deleted</span></span>|<span data-ttu-id="ec072-131">6</span><span class="sxs-lookup"><span data-stu-id="ec072-131">6</span></span>|<span data-ttu-id="ec072-132">デバイスからプロファイルを削除することを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec072-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="ec072-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="ec072-133">removedByUser</span></span>|<span data-ttu-id="ec072-134">7</span><span class="sxs-lookup"><span data-stu-id="ec072-134">7</span></span>|<span data-ttu-id="ec072-135">ユーザーがデバイスからプロファイルが削除されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="ec072-135">Designates that the profile is removed from the device by the user</span></span>|





