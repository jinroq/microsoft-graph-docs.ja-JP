---
title: embeddedSIMDeviceStateValue 列挙型
description: 埋め込まれた SIM のアクティブ化コードのさまざまな状態について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a4970e08ff9b305aaf2aad4d82daf994d2010bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568767"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a><span data-ttu-id="e201f-103">embeddedSIMDeviceStateValue 列挙型</span><span class="sxs-lookup"><span data-stu-id="e201f-103">embeddedSIMDeviceStateValue enum type</span></span>

> <span data-ttu-id="e201f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e201f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e201f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e201f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e201f-106">埋め込まれた SIM のアクティブ化コードのさまざまな状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="e201f-106">Describes the various states for an embedded SIM activation code.</span></span>

## <a name="members"></a><span data-ttu-id="e201f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e201f-107">Members</span></span>
|<span data-ttu-id="e201f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e201f-108">Member</span></span>|<span data-ttu-id="e201f-109">値</span><span class="sxs-lookup"><span data-stu-id="e201f-109">Value</span></span>|<span data-ttu-id="e201f-110">説明</span><span class="sxs-lookup"><span data-stu-id="e201f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e201f-111">注評価</span><span class="sxs-lookup"><span data-stu-id="e201f-111">notEvaluated</span></span>|<span data-ttu-id="e201f-112">.0</span><span class="sxs-lookup"><span data-stu-id="e201f-112">0</span></span>|<span data-ttu-id="e201f-113">埋め込まれている SIM ライセンス認証コードが無料で、デバイスに割り当てることができることを指定します。</span><span class="sxs-lookup"><span data-stu-id="e201f-113">Designates that the embedded SIM activation code is free and available to be assigned to a device.</span></span>|
|<span data-ttu-id="e201f-114">フェール</span><span class="sxs-lookup"><span data-stu-id="e201f-114">failed</span></span>|<span data-ttu-id="e201f-115">1 </span><span class="sxs-lookup"><span data-stu-id="e201f-115">1</span></span>|<span data-ttu-id="e201f-116">Intune サービスがこのプロファイルをデバイスに配信できなかったことを指定します。</span><span class="sxs-lookup"><span data-stu-id="e201f-116">Designates that Intune Service failed to deliver this profile to a device.</span></span>|
|<span data-ttu-id="e201f-117">インストール</span><span class="sxs-lookup"><span data-stu-id="e201f-117">installing</span></span>|<span data-ttu-id="e201f-118">2 </span><span class="sxs-lookup"><span data-stu-id="e201f-118">2</span></span>|<span data-ttu-id="e201f-119">埋め込まれた SIM ライセンス認証コードがデバイスに割り当てられており、デバイスがトークンをインストールしていることを指定します。</span><span class="sxs-lookup"><span data-stu-id="e201f-119">Designates that the embedded SIM activation code has been assigned to a device and the device is installing the token.</span></span>|
|<span data-ttu-id="e201f-120">れる</span><span class="sxs-lookup"><span data-stu-id="e201f-120">installed</span></span>|<span data-ttu-id="e201f-121">3 </span><span class="sxs-lookup"><span data-stu-id="e201f-121">3</span></span>|<span data-ttu-id="e201f-122">埋め込まれた SIM ライセンス認証コードがターゲットデバイスに正常にインストールされたことを指定します。</span><span class="sxs-lookup"><span data-stu-id="e201f-122">Designates that the embedded SIM activation code has been successfully installed on the target device.</span></span>|
|<span data-ttu-id="e201f-123">と</span><span class="sxs-lookup"><span data-stu-id="e201f-123">deleting</span></span>|<span data-ttu-id="e201f-124">4 </span><span class="sxs-lookup"><span data-stu-id="e201f-124">4</span></span>|<span data-ttu-id="e201f-125">Intune サービスがデバイスからプロファイルを削除しようとしていることを指定します。</span><span class="sxs-lookup"><span data-stu-id="e201f-125">Designates that Intune Service is trying to delete the profile from the device.</span></span>|
|<span data-ttu-id="e201f-126">error</span><span class="sxs-lookup"><span data-stu-id="e201f-126">error</span></span>|<span data-ttu-id="e201f-127">5 </span><span class="sxs-lookup"><span data-stu-id="e201f-127">5</span></span>|<span data-ttu-id="e201f-128">このプロファイルにエラーがあることを指定します。</span><span class="sxs-lookup"><span data-stu-id="e201f-128">Designates that there is error with this profile.</span></span>|
|<span data-ttu-id="e201f-129">deleted</span><span class="sxs-lookup"><span data-stu-id="e201f-129">deleted</span></span>|<span data-ttu-id="e201f-130">6 </span><span class="sxs-lookup"><span data-stu-id="e201f-130">6</span></span>|<span data-ttu-id="e201f-131">プロファイルがデバイスから削除されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="e201f-131">Designates that the profile is deleted from the device.</span></span>|
|<span data-ttu-id="e201f-132">removedbyuser</span><span class="sxs-lookup"><span data-stu-id="e201f-132">removedByUser</span></span>|<span data-ttu-id="e201f-133">7 </span><span class="sxs-lookup"><span data-stu-id="e201f-133">7</span></span>|<span data-ttu-id="e201f-134">ユーザーがプロファイルをデバイスから削除することを指定します。</span><span class="sxs-lookup"><span data-stu-id="e201f-134">Designates that the profile is removed from the device by the user</span></span>|





