---
title: embeddedSIMDeviceStateValue 列挙型
description: SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421327"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="22c2c-103">embeddedSIMDeviceStateValue 列挙型</span><span class="sxs-lookup"><span data-stu-id="22c2c-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="22c2c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22c2c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22c2c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22c2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22c2c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22c2c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22c2c-107">SIM の埋め込みのライセンス認証コードのさまざまな状態をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-107">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="22c2c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="22c2c-108">Members</span></span>
|<span data-ttu-id="22c2c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="22c2c-109">Member</span></span>|<span data-ttu-id="22c2c-110">値</span><span class="sxs-lookup"><span data-stu-id="22c2c-110">Value</span></span>|<span data-ttu-id="22c2c-111">説明</span><span class="sxs-lookup"><span data-stu-id="22c2c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22c2c-112">notEvaluated</span><span class="sxs-lookup"><span data-stu-id="22c2c-112">notEvaluated</span></span>|<span data-ttu-id="22c2c-113">0</span><span class="sxs-lookup"><span data-stu-id="22c2c-113">0</span></span>|<span data-ttu-id="22c2c-114">SIM の埋め込みのライセンス認証コードが空き時間と、デバイスに割り当てられる利用可能なことを指定します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-114">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="22c2c-115">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="22c2c-115">failed</span></span>|<span data-ttu-id="22c2c-116">1</span><span class="sxs-lookup"><span data-stu-id="22c2c-116">1</span></span>|<span data-ttu-id="22c2c-117">Intune サービスがデバイスにこのプロファイルを提供する失敗したことを指定します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-117">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="22c2c-118">インストール</span><span class="sxs-lookup"><span data-stu-id="22c2c-118">installing</span></span>|<span data-ttu-id="22c2c-119">2</span><span class="sxs-lookup"><span data-stu-id="22c2c-119">2</span></span>|<span data-ttu-id="22c2c-120">SIM の埋め込みのライセンス認証コードは、デバイスに割り当てられているし、デバイスが、トークンをインストールすることを指定します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-120">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="22c2c-121">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="22c2c-121">installed</span></span>|<span data-ttu-id="22c2c-122">3</span><span class="sxs-lookup"><span data-stu-id="22c2c-122">3</span></span>|<span data-ttu-id="22c2c-123">SIM の埋め込みのライセンス認証コードがターゲット ・ デバイスを正常にインストールされているかを指定します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-123">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="22c2c-124">削除</span><span class="sxs-lookup"><span data-stu-id="22c2c-124">deleting</span></span>|<span data-ttu-id="22c2c-125">4</span><span class="sxs-lookup"><span data-stu-id="22c2c-125">4</span></span>|<span data-ttu-id="22c2c-126">Intune サービスがデバイスのプロファイルを削除しようとしていることを指定します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-126">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="22c2c-127">エラー</span><span class="sxs-lookup"><span data-stu-id="22c2c-127">error</span></span>|<span data-ttu-id="22c2c-128">5</span><span class="sxs-lookup"><span data-stu-id="22c2c-128">5</span></span>|<span data-ttu-id="22c2c-129">このプロファイルを使用してエラーがあることを指定します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-129">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="22c2c-130">deleted</span><span class="sxs-lookup"><span data-stu-id="22c2c-130">deleted</span></span>|<span data-ttu-id="22c2c-131">6</span><span class="sxs-lookup"><span data-stu-id="22c2c-131">6</span></span>|<span data-ttu-id="22c2c-132">デバイスからプロファイルを削除することを指定します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-132">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="22c2c-133">removedByUser</span><span class="sxs-lookup"><span data-stu-id="22c2c-133">removedByUser</span></span>|<span data-ttu-id="22c2c-134">7</span><span class="sxs-lookup"><span data-stu-id="22c2c-134">7</span></span>|<span data-ttu-id="22c2c-135">ユーザーがデバイスからプロファイルが削除されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="22c2c-135">Designates that the profile is removed from the device by the user</span></span>|




