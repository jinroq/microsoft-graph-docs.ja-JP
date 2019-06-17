---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange アクセス状態の理由。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10482c09f7aa7dcf22b6091e55e74f4bd53b0c60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983023"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="69e43-103">deviceManagementExchangeAccessStateReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="69e43-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="69e43-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69e43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69e43-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="69e43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69e43-106">デバイスの Exchange アクセス状態の理由。</span><span class="sxs-lookup"><span data-stu-id="69e43-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="69e43-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="69e43-107">Members</span></span>
|<span data-ttu-id="69e43-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="69e43-108">Member</span></span>|<span data-ttu-id="69e43-109">値</span><span class="sxs-lookup"><span data-stu-id="69e43-109">Value</span></span>|<span data-ttu-id="69e43-110">説明</span><span class="sxs-lookup"><span data-stu-id="69e43-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69e43-111">none</span><span class="sxs-lookup"><span data-stu-id="69e43-111">none</span></span>|<span data-ttu-id="69e43-112">.0</span><span class="sxs-lookup"><span data-stu-id="69e43-112">0</span></span>|<span data-ttu-id="69e43-113">Exchange から検出されたアクセス状態の理由はありません</span><span class="sxs-lookup"><span data-stu-id="69e43-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="69e43-114">不明</span><span class="sxs-lookup"><span data-stu-id="69e43-114">unknown</span></span>|<span data-ttu-id="69e43-115">1-d</span><span class="sxs-lookup"><span data-stu-id="69e43-115">1</span></span>|<span data-ttu-id="69e43-116">不明なアクセス状態の理由</span><span class="sxs-lookup"><span data-stu-id="69e43-116">Unknown access state reason</span></span>|
|<span data-ttu-id="69e43-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="69e43-117">exchangeGlobalRule</span></span>|<span data-ttu-id="69e43-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="69e43-118">2</span></span>|<span data-ttu-id="69e43-119">Exchange グローバルルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="69e43-120">Exchange個性 Alrule</span><span class="sxs-lookup"><span data-stu-id="69e43-120">exchangeIndividualRule</span></span>|<span data-ttu-id="69e43-121">1/3</span><span class="sxs-lookup"><span data-stu-id="69e43-121">3</span></span>|<span data-ttu-id="69e43-122">Exchange の個々のルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="69e43-123">exchangeDeviceRule 方法</span><span class="sxs-lookup"><span data-stu-id="69e43-123">exchangeDeviceRule</span></span>|<span data-ttu-id="69e43-124">2/4</span><span class="sxs-lookup"><span data-stu-id="69e43-124">4</span></span>|<span data-ttu-id="69e43-125">Exchange デバイスルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="69e43-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="69e43-126">exchangeUpgrade</span></span>|<span data-ttu-id="69e43-127">5</span><span class="sxs-lookup"><span data-stu-id="69e43-127">5</span></span>|<span data-ttu-id="69e43-128">Exchange アップグレードのためのアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="69e43-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="69e43-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="69e43-130">シックス</span><span class="sxs-lookup"><span data-stu-id="69e43-130">6</span></span>|<span data-ttu-id="69e43-131">Exchange メールボックスポリシーによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="69e43-132">も</span><span class="sxs-lookup"><span data-stu-id="69e43-132">other</span></span>|<span data-ttu-id="69e43-133">7</span><span class="sxs-lookup"><span data-stu-id="69e43-133">7</span></span>|<span data-ttu-id="69e43-134">Exchange によって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="69e43-135">要件</span><span class="sxs-lookup"><span data-stu-id="69e43-135">compliant</span></span>|<span data-ttu-id="69e43-136">8 </span><span class="sxs-lookup"><span data-stu-id="69e43-136">8</span></span>|<span data-ttu-id="69e43-137">コンプライアンスの課題によって付与されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="69e43-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="69e43-138">notCompliant</span></span>|<span data-ttu-id="69e43-139">9 </span><span class="sxs-lookup"><span data-stu-id="69e43-139">9</span></span>|<span data-ttu-id="69e43-140">コンプライアンスの課題によるアクセス状態の取り消し</span><span class="sxs-lookup"><span data-stu-id="69e43-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="69e43-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="69e43-141">notEnrolled</span></span>|<span data-ttu-id="69e43-142">10 </span><span class="sxs-lookup"><span data-stu-id="69e43-142">10</span></span>|<span data-ttu-id="69e43-143">管理の課題によるアクセス状態の取り消し</span><span class="sxs-lookup"><span data-stu-id="69e43-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="69e43-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="69e43-144">unknownLocation</span></span>|<span data-ttu-id="69e43-145">個</span><span class="sxs-lookup"><span data-stu-id="69e43-145">12</span></span>|<span data-ttu-id="69e43-146">不明な場所のためのアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="69e43-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="69e43-147">mfaRequired</span></span>|<span data-ttu-id="69e43-148">スリー</span><span class="sxs-lookup"><span data-stu-id="69e43-148">13</span></span>|<span data-ttu-id="69e43-149">MFA チャレンジによるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="69e43-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="69e43-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="69e43-151">第</span><span class="sxs-lookup"><span data-stu-id="69e43-151">14</span></span>|<span data-ttu-id="69e43-152">AAD アクセスポリシーによって無効にされたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="69e43-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="69e43-153">compromisedPassword</span></span>|<span data-ttu-id="69e43-154">約</span><span class="sxs-lookup"><span data-stu-id="69e43-154">15</span></span>|<span data-ttu-id="69e43-155">侵害されたパスワードによって取り消されたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="69e43-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="69e43-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="69e43-157">16</span><span class="sxs-lookup"><span data-stu-id="69e43-157">16</span></span>|<span data-ttu-id="69e43-158">管理対象アプリケーションのチャレンジによって取り消されたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="69e43-158">Access state revoked by managed application challenge</span></span>|





