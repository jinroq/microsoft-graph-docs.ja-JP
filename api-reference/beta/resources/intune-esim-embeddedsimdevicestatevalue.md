---
title: embeddedSIMDeviceStateValue 列挙型
description: 埋め込まれた SIM のアクティブ化コードのさまざまな状態について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a4970e08ff9b305aaf2aad4d82daf994d2010bc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782962"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="fd5c5-103">embeddedSIMDeviceStateValue 列挙型</span><span class="sxs-lookup"><span data-stu-id="fd5c5-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="fd5c5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd5c5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd5c5-106">埋め込まれた SIM のアクティブ化コードのさまざまな状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="fd5c5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="fd5c5-107">Members</span></span>
|<span data-ttu-id="fd5c5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fd5c5-108">Member</span></span>|<span data-ttu-id="fd5c5-109">値</span><span class="sxs-lookup"><span data-stu-id="fd5c5-109">Value</span></span>|<span data-ttu-id="fd5c5-110">説明</span><span class="sxs-lookup"><span data-stu-id="fd5c5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd5c5-111">注評価</span><span class="sxs-lookup"><span data-stu-id="fd5c5-111">notEvaluated</span></span>|<span data-ttu-id="fd5c5-112">.0</span><span class="sxs-lookup"><span data-stu-id="fd5c5-112">0</span></span>|<span data-ttu-id="fd5c5-113">埋め込まれている SIM ライセンス認証コードが無料で、デバイスに割り当てることができることを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="fd5c5-114">フェール</span><span class="sxs-lookup"><span data-stu-id="fd5c5-114">failed</span></span>|<span data-ttu-id="fd5c5-115">1-d</span><span class="sxs-lookup"><span data-stu-id="fd5c5-115">1</span></span>|<span data-ttu-id="fd5c5-116">Intune サービスがこのプロファイルをデバイスに配信できなかったことを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="fd5c5-117">インストール</span><span class="sxs-lookup"><span data-stu-id="fd5c5-117">installing</span></span>|<span data-ttu-id="fd5c5-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="fd5c5-118">2</span></span>|<span data-ttu-id="fd5c5-119">埋め込まれた SIM ライセンス認証コードがデバイスに割り当てられており、デバイスがトークンをインストールしていることを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="fd5c5-120">れる</span><span class="sxs-lookup"><span data-stu-id="fd5c5-120">installed</span></span>|<span data-ttu-id="fd5c5-121">1/3</span><span class="sxs-lookup"><span data-stu-id="fd5c5-121">3</span></span>|<span data-ttu-id="fd5c5-122">埋め込まれた SIM ライセンス認証コードがターゲットデバイスに正常にインストールされたことを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="fd5c5-123">と</span><span class="sxs-lookup"><span data-stu-id="fd5c5-123">deleting</span></span>|<span data-ttu-id="fd5c5-124">2/4</span><span class="sxs-lookup"><span data-stu-id="fd5c5-124">4</span></span>|<span data-ttu-id="fd5c5-125">Intune サービスがデバイスからプロファイルを削除しようとしていることを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="fd5c5-126">エラー</span><span class="sxs-lookup"><span data-stu-id="fd5c5-126">error</span></span>|<span data-ttu-id="fd5c5-127">5</span><span class="sxs-lookup"><span data-stu-id="fd5c5-127">5</span></span>|<span data-ttu-id="fd5c5-128">このプロファイルにエラーがあることを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="fd5c5-129">deleted</span><span class="sxs-lookup"><span data-stu-id="fd5c5-129">deleted</span></span>|<span data-ttu-id="fd5c5-130">シックス</span><span class="sxs-lookup"><span data-stu-id="fd5c5-130">6</span></span>|<span data-ttu-id="fd5c5-131">プロファイルがデバイスから削除されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="fd5c5-132">removedbyuser</span><span class="sxs-lookup"><span data-stu-id="fd5c5-132">removedByUser</span></span>|<span data-ttu-id="fd5c5-133">7</span><span class="sxs-lookup"><span data-stu-id="fd5c5-133">7</span></span>|<span data-ttu-id="fd5c5-134">ユーザーがプロファイルをデバイスから削除することを指定します。</span><span class="sxs-lookup"><span data-stu-id="fd5c5-134">Designates that the profile is removed from the device by the user</span></span>|





