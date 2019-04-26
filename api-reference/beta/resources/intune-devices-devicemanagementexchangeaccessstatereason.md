---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange アクセス状態の理由。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dab2b0b39290568331a16473fd6eaf7286ce5df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570048"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="79363-103">deviceManagementExchangeAccessStateReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="79363-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="79363-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79363-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79363-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79363-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79363-106">デバイスの Exchange アクセス状態の理由。</span><span class="sxs-lookup"><span data-stu-id="79363-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="79363-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="79363-107">Members</span></span>
|<span data-ttu-id="79363-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="79363-108">Member</span></span>|<span data-ttu-id="79363-109">値</span><span class="sxs-lookup"><span data-stu-id="79363-109">Value</span></span>|<span data-ttu-id="79363-110">説明</span><span class="sxs-lookup"><span data-stu-id="79363-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79363-111">なし</span><span class="sxs-lookup"><span data-stu-id="79363-111">none</span></span>|<span data-ttu-id="79363-112">.0</span><span class="sxs-lookup"><span data-stu-id="79363-112">0</span></span>|<span data-ttu-id="79363-113">Exchange から検出されたアクセス状態の理由はありません</span><span class="sxs-lookup"><span data-stu-id="79363-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="79363-114">不明</span><span class="sxs-lookup"><span data-stu-id="79363-114">unknown</span></span>|<span data-ttu-id="79363-115">1 </span><span class="sxs-lookup"><span data-stu-id="79363-115">1</span></span>|<span data-ttu-id="79363-116">不明なアクセス状態の理由</span><span class="sxs-lookup"><span data-stu-id="79363-116">Unknown access state reason</span></span>|
|<span data-ttu-id="79363-117">exchangeglobalrule</span><span class="sxs-lookup"><span data-stu-id="79363-117">exchangeGlobalRule</span></span>|<span data-ttu-id="79363-118">2 </span><span class="sxs-lookup"><span data-stu-id="79363-118">2</span></span>|<span data-ttu-id="79363-119">Exchange グローバルルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="79363-120">exchange個性 alrule</span><span class="sxs-lookup"><span data-stu-id="79363-120">exchangeIndividualRule</span></span>|<span data-ttu-id="79363-121">3 </span><span class="sxs-lookup"><span data-stu-id="79363-121">3</span></span>|<span data-ttu-id="79363-122">Exchange の個々のルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="79363-123">exchangedevicerule 方法</span><span class="sxs-lookup"><span data-stu-id="79363-123">exchangeDeviceRule</span></span>|<span data-ttu-id="79363-124">4 </span><span class="sxs-lookup"><span data-stu-id="79363-124">4</span></span>|<span data-ttu-id="79363-125">Exchange デバイスルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="79363-126">exchangeupgrade</span><span class="sxs-lookup"><span data-stu-id="79363-126">exchangeUpgrade</span></span>|<span data-ttu-id="79363-127">5 </span><span class="sxs-lookup"><span data-stu-id="79363-127">5</span></span>|<span data-ttu-id="79363-128">Exchange アップグレードのためのアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="79363-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="79363-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="79363-130">6 </span><span class="sxs-lookup"><span data-stu-id="79363-130">6</span></span>|<span data-ttu-id="79363-131">Exchange メールボックスポリシーによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="79363-132">も</span><span class="sxs-lookup"><span data-stu-id="79363-132">other</span></span>|<span data-ttu-id="79363-133">7 </span><span class="sxs-lookup"><span data-stu-id="79363-133">7</span></span>|<span data-ttu-id="79363-134">Exchange によって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="79363-135">要件</span><span class="sxs-lookup"><span data-stu-id="79363-135">compliant</span></span>|<span data-ttu-id="79363-136">8 </span><span class="sxs-lookup"><span data-stu-id="79363-136">8</span></span>|<span data-ttu-id="79363-137">コンプライアンスの課題によって付与されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="79363-138">notcompliant</span><span class="sxs-lookup"><span data-stu-id="79363-138">notCompliant</span></span>|<span data-ttu-id="79363-139">9 </span><span class="sxs-lookup"><span data-stu-id="79363-139">9</span></span>|<span data-ttu-id="79363-140">コンプライアンスの課題によるアクセス状態の取り消し</span><span class="sxs-lookup"><span data-stu-id="79363-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="79363-141">notenrolled</span><span class="sxs-lookup"><span data-stu-id="79363-141">notEnrolled</span></span>|<span data-ttu-id="79363-142">10  </span><span class="sxs-lookup"><span data-stu-id="79363-142">10</span></span>|<span data-ttu-id="79363-143">管理の課題によるアクセス状態の取り消し</span><span class="sxs-lookup"><span data-stu-id="79363-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="79363-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="79363-144">unknownLocation</span></span>|<span data-ttu-id="79363-145">12 </span><span class="sxs-lookup"><span data-stu-id="79363-145">12</span></span>|<span data-ttu-id="79363-146">不明な場所のためのアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="79363-147">mfarequired</span><span class="sxs-lookup"><span data-stu-id="79363-147">mfaRequired</span></span>|<span data-ttu-id="79363-148">13 </span><span class="sxs-lookup"><span data-stu-id="79363-148">13</span></span>|<span data-ttu-id="79363-149">MFA チャレンジによるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="79363-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="79363-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="79363-151">14 </span><span class="sxs-lookup"><span data-stu-id="79363-151">14</span></span>|<span data-ttu-id="79363-152">AAD アクセスポリシーによって無効にされたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="79363-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="79363-153">compromisedPassword</span></span>|<span data-ttu-id="79363-154">15 </span><span class="sxs-lookup"><span data-stu-id="79363-154">15</span></span>|<span data-ttu-id="79363-155">侵害されたパスワードによって取り消されたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="79363-156">devicenotknownwithmanagedapp</span><span class="sxs-lookup"><span data-stu-id="79363-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="79363-157">16 </span><span class="sxs-lookup"><span data-stu-id="79363-157">16</span></span>|<span data-ttu-id="79363-158">管理対象アプリケーションのチャレンジによって取り消されたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="79363-158">Access state revoked by managed application challenge</span></span>|





