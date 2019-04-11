---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange アクセス状態の理由。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dab2b0b39290568331a16473fd6eaf7286ce5df
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794401"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="e4198-103">deviceManagementExchangeAccessStateReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="e4198-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="e4198-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4198-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4198-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e4198-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4198-106">デバイスの Exchange アクセス状態の理由。</span><span class="sxs-lookup"><span data-stu-id="e4198-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="e4198-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e4198-107">Members</span></span>
|<span data-ttu-id="e4198-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e4198-108">Member</span></span>|<span data-ttu-id="e4198-109">値</span><span class="sxs-lookup"><span data-stu-id="e4198-109">Value</span></span>|<span data-ttu-id="e4198-110">説明</span><span class="sxs-lookup"><span data-stu-id="e4198-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4198-111">none</span><span class="sxs-lookup"><span data-stu-id="e4198-111">none</span></span>|<span data-ttu-id="e4198-112">.0</span><span class="sxs-lookup"><span data-stu-id="e4198-112">0</span></span>|<span data-ttu-id="e4198-113">Exchange から検出されたアクセス状態の理由はありません</span><span class="sxs-lookup"><span data-stu-id="e4198-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="e4198-114">不明</span><span class="sxs-lookup"><span data-stu-id="e4198-114">unknown</span></span>|<span data-ttu-id="e4198-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e4198-115">1</span></span>|<span data-ttu-id="e4198-116">不明なアクセス状態の理由</span><span class="sxs-lookup"><span data-stu-id="e4198-116">Unknown access state reason</span></span>|
|<span data-ttu-id="e4198-117">exchangeglobalrule</span><span class="sxs-lookup"><span data-stu-id="e4198-117">exchangeGlobalRule</span></span>|<span data-ttu-id="e4198-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e4198-118">2</span></span>|<span data-ttu-id="e4198-119">Exchange グローバルルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="e4198-120">exchange個性 alrule</span><span class="sxs-lookup"><span data-stu-id="e4198-120">exchangeIndividualRule</span></span>|<span data-ttu-id="e4198-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e4198-121">3</span></span>|<span data-ttu-id="e4198-122">Exchange の個々のルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="e4198-123">exchangedevicerule 方法</span><span class="sxs-lookup"><span data-stu-id="e4198-123">exchangeDeviceRule</span></span>|<span data-ttu-id="e4198-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e4198-124">4</span></span>|<span data-ttu-id="e4198-125">Exchange デバイスルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="e4198-126">exchangeupgrade</span><span class="sxs-lookup"><span data-stu-id="e4198-126">exchangeUpgrade</span></span>|<span data-ttu-id="e4198-127">5</span><span class="sxs-lookup"><span data-stu-id="e4198-127">5</span></span>|<span data-ttu-id="e4198-128">Exchange アップグレードのためのアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="e4198-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="e4198-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="e4198-130">シックス</span><span class="sxs-lookup"><span data-stu-id="e4198-130">6</span></span>|<span data-ttu-id="e4198-131">Exchange メールボックスポリシーによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="e4198-132">も</span><span class="sxs-lookup"><span data-stu-id="e4198-132">other</span></span>|<span data-ttu-id="e4198-133">7</span><span class="sxs-lookup"><span data-stu-id="e4198-133">7</span></span>|<span data-ttu-id="e4198-134">Exchange によって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="e4198-135">要件</span><span class="sxs-lookup"><span data-stu-id="e4198-135">compliant</span></span>|<span data-ttu-id="e4198-136">~</span><span class="sxs-lookup"><span data-stu-id="e4198-136">8</span></span>|<span data-ttu-id="e4198-137">コンプライアンスの課題によって付与されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="e4198-138">notcompliant</span><span class="sxs-lookup"><span data-stu-id="e4198-138">notCompliant</span></span>|<span data-ttu-id="e4198-139">i-9</span><span class="sxs-lookup"><span data-stu-id="e4198-139">9</span></span>|<span data-ttu-id="e4198-140">コンプライアンスの課題によるアクセス状態の取り消し</span><span class="sxs-lookup"><span data-stu-id="e4198-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="e4198-141">notenrolled</span><span class="sxs-lookup"><span data-stu-id="e4198-141">notEnrolled</span></span>|<span data-ttu-id="e4198-142">個</span><span class="sxs-lookup"><span data-stu-id="e4198-142">10</span></span>|<span data-ttu-id="e4198-143">管理の課題によるアクセス状態の取り消し</span><span class="sxs-lookup"><span data-stu-id="e4198-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="e4198-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="e4198-144">unknownLocation</span></span>|<span data-ttu-id="e4198-145">個</span><span class="sxs-lookup"><span data-stu-id="e4198-145">12</span></span>|<span data-ttu-id="e4198-146">不明な場所のためのアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="e4198-147">mfarequired</span><span class="sxs-lookup"><span data-stu-id="e4198-147">mfaRequired</span></span>|<span data-ttu-id="e4198-148">スリー</span><span class="sxs-lookup"><span data-stu-id="e4198-148">13</span></span>|<span data-ttu-id="e4198-149">MFA チャレンジによるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="e4198-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e4198-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="e4198-151">第</span><span class="sxs-lookup"><span data-stu-id="e4198-151">14</span></span>|<span data-ttu-id="e4198-152">AAD アクセスポリシーによって無効にされたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="e4198-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="e4198-153">compromisedPassword</span></span>|<span data-ttu-id="e4198-154">約</span><span class="sxs-lookup"><span data-stu-id="e4198-154">15</span></span>|<span data-ttu-id="e4198-155">侵害されたパスワードによって取り消されたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="e4198-156">devicenotknownwithmanagedapp</span><span class="sxs-lookup"><span data-stu-id="e4198-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="e4198-157">16</span><span class="sxs-lookup"><span data-stu-id="e4198-157">16</span></span>|<span data-ttu-id="e4198-158">管理対象アプリケーションのチャレンジによって取り消されたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="e4198-158">Access state revoked by managed application challenge</span></span>|





