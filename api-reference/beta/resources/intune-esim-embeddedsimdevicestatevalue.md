---
title: embeddedSIMDeviceStateValue 列挙型
description: SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。
ms.openlocfilehash: c0b1cffedcae18dab4c1d23a2691cafa8709c0ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067589"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="62307-103">embeddedSIMDeviceStateValue 列挙型</span><span class="sxs-lookup"><span data-stu-id="62307-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="62307-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="62307-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62307-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62307-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62307-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="62307-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62307-107">SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="62307-107">Describes the various states for an embedded SIM activation code.</span></span>
## <a name="members"></a><span data-ttu-id="62307-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="62307-108">Members</span></span>
|<span data-ttu-id="62307-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="62307-109">Member</span></span>|<span data-ttu-id="62307-110">値</span><span class="sxs-lookup"><span data-stu-id="62307-110">Value</span></span>|<span data-ttu-id="62307-111">説明</span><span class="sxs-lookup"><span data-stu-id="62307-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62307-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="62307-112">notEvaluated</span></span>|<span data-ttu-id="62307-113">0</span><span class="sxs-lookup"><span data-stu-id="62307-113">0</span></span>|<span data-ttu-id="62307-114">SIM の埋め込みのライセンス認証コードが空き時間と、デバイスに割り当てられる利用可能なことを指定します。</span><span class="sxs-lookup"><span data-stu-id="62307-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="62307-115">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="62307-115">failed</span></span>|<span data-ttu-id="62307-116">1</span><span class="sxs-lookup"><span data-stu-id="62307-116">1</span></span>|<span data-ttu-id="62307-117">Intune サービスがデバイスにこのプロファイルを提供する失敗したことを指定します。</span><span class="sxs-lookup"><span data-stu-id="62307-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="62307-118">インストール</span><span class="sxs-lookup"><span data-stu-id="62307-118">installing</span></span>|<span data-ttu-id="62307-119">2</span><span class="sxs-lookup"><span data-stu-id="62307-119">2</span></span>|<span data-ttu-id="62307-120">SIM の埋め込みのライセンス認証コードは、デバイスに割り当てられているし、デバイスが、トークンをインストールすることを指定します。</span><span class="sxs-lookup"><span data-stu-id="62307-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="62307-121">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="62307-121">installed</span></span>|<span data-ttu-id="62307-122">3</span><span class="sxs-lookup"><span data-stu-id="62307-122">3</span></span>|<span data-ttu-id="62307-123">SIM の埋め込みのライセンス認証コードがターゲット ・ デバイスを正常にインストールされているかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62307-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="62307-124">削除</span><span class="sxs-lookup"><span data-stu-id="62307-124">deleting</span></span>|<span data-ttu-id="62307-125">4</span><span class="sxs-lookup"><span data-stu-id="62307-125">4</span></span>|<span data-ttu-id="62307-126">Intune サービスがデバイスのプロファイルを削除しようとしていることを指定します。</span><span class="sxs-lookup"><span data-stu-id="62307-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="62307-127">エラー</span><span class="sxs-lookup"><span data-stu-id="62307-127">error</span></span>|<span data-ttu-id="62307-128">5</span><span class="sxs-lookup"><span data-stu-id="62307-128">5</span></span>|<span data-ttu-id="62307-129">このプロファイルを使用してエラーがあることを指定します。</span><span class="sxs-lookup"><span data-stu-id="62307-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="62307-130">deleted</span><span class="sxs-lookup"><span data-stu-id="62307-130">deleted</span></span>|<span data-ttu-id="62307-131">6</span><span class="sxs-lookup"><span data-stu-id="62307-131">6</span></span>|<span data-ttu-id="62307-132">デバイスからプロファイルを削除することを指定します。</span><span class="sxs-lookup"><span data-stu-id="62307-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="62307-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="62307-133">removedByUser</span></span>|<span data-ttu-id="62307-134">7</span><span class="sxs-lookup"><span data-stu-id="62307-134">7</span></span>|<span data-ttu-id="62307-135">ユーザーがデバイスからプロファイルが削除されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="62307-135">Designates that the profile is removed from the device by the user</span></span>|





