---
title: deviceManagementExchangeAccessStateReason 列挙型
description: デバイスの Exchange アクセス状態の理由。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d6761af448b51c9c434472c4ad43978d34b1b1b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968463"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="afb6c-103">deviceManagementExchangeAccessStateReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="afb6c-103">deviceManagementExchangeAccessStateReason enum type</span></span>

> <span data-ttu-id="afb6c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afb6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afb6c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="afb6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afb6c-106">デバイスの Exchange アクセス状態の理由。</span><span class="sxs-lookup"><span data-stu-id="afb6c-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="afb6c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="afb6c-107">Members</span></span>
|<span data-ttu-id="afb6c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="afb6c-108">Member</span></span>|<span data-ttu-id="afb6c-109">値</span><span class="sxs-lookup"><span data-stu-id="afb6c-109">Value</span></span>|<span data-ttu-id="afb6c-110">説明</span><span class="sxs-lookup"><span data-stu-id="afb6c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afb6c-111">none</span><span class="sxs-lookup"><span data-stu-id="afb6c-111">none</span></span>|<span data-ttu-id="afb6c-112">.0</span><span class="sxs-lookup"><span data-stu-id="afb6c-112">0</span></span>|<span data-ttu-id="afb6c-113">Exchange から検出されたアクセス状態の理由はありません</span><span class="sxs-lookup"><span data-stu-id="afb6c-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="afb6c-114">不明</span><span class="sxs-lookup"><span data-stu-id="afb6c-114">unknown</span></span>|<span data-ttu-id="afb6c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="afb6c-115">1</span></span>|<span data-ttu-id="afb6c-116">不明なアクセス状態の理由</span><span class="sxs-lookup"><span data-stu-id="afb6c-116">Unknown access state reason</span></span>|
|<span data-ttu-id="afb6c-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="afb6c-117">exchangeGlobalRule</span></span>|<span data-ttu-id="afb6c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="afb6c-118">2</span></span>|<span data-ttu-id="afb6c-119">Exchange グローバルルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="afb6c-120">Exchange個性 Alrule</span><span class="sxs-lookup"><span data-stu-id="afb6c-120">exchangeIndividualRule</span></span>|<span data-ttu-id="afb6c-121">1/3</span><span class="sxs-lookup"><span data-stu-id="afb6c-121">3</span></span>|<span data-ttu-id="afb6c-122">Exchange の個々のルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="afb6c-123">exchangeDeviceRule 方法</span><span class="sxs-lookup"><span data-stu-id="afb6c-123">exchangeDeviceRule</span></span>|<span data-ttu-id="afb6c-124">2/4</span><span class="sxs-lookup"><span data-stu-id="afb6c-124">4</span></span>|<span data-ttu-id="afb6c-125">Exchange デバイスルールによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="afb6c-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="afb6c-126">exchangeUpgrade</span></span>|<span data-ttu-id="afb6c-127">5</span><span class="sxs-lookup"><span data-stu-id="afb6c-127">5</span></span>|<span data-ttu-id="afb6c-128">Exchange アップグレードのためのアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="afb6c-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="afb6c-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="afb6c-130">シックス</span><span class="sxs-lookup"><span data-stu-id="afb6c-130">6</span></span>|<span data-ttu-id="afb6c-131">Exchange メールボックスポリシーによって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="afb6c-132">も</span><span class="sxs-lookup"><span data-stu-id="afb6c-132">other</span></span>|<span data-ttu-id="afb6c-133">7</span><span class="sxs-lookup"><span data-stu-id="afb6c-133">7</span></span>|<span data-ttu-id="afb6c-134">Exchange によって決定されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="afb6c-135">要件</span><span class="sxs-lookup"><span data-stu-id="afb6c-135">compliant</span></span>|<span data-ttu-id="afb6c-136">8 </span><span class="sxs-lookup"><span data-stu-id="afb6c-136">8</span></span>|<span data-ttu-id="afb6c-137">コンプライアンスの課題によって付与されるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="afb6c-138">notCompliant</span><span class="sxs-lookup"><span data-stu-id="afb6c-138">notCompliant</span></span>|<span data-ttu-id="afb6c-139">9 </span><span class="sxs-lookup"><span data-stu-id="afb6c-139">9</span></span>|<span data-ttu-id="afb6c-140">コンプライアンスの課題によるアクセス状態の取り消し</span><span class="sxs-lookup"><span data-stu-id="afb6c-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="afb6c-141">notEnrolled</span><span class="sxs-lookup"><span data-stu-id="afb6c-141">notEnrolled</span></span>|<span data-ttu-id="afb6c-142">10 </span><span class="sxs-lookup"><span data-stu-id="afb6c-142">10</span></span>|<span data-ttu-id="afb6c-143">管理の課題によるアクセス状態の取り消し</span><span class="sxs-lookup"><span data-stu-id="afb6c-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="afb6c-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="afb6c-144">unknownLocation</span></span>|<span data-ttu-id="afb6c-145">個</span><span class="sxs-lookup"><span data-stu-id="afb6c-145">12</span></span>|<span data-ttu-id="afb6c-146">不明な場所のためのアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="afb6c-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="afb6c-147">mfaRequired</span></span>|<span data-ttu-id="afb6c-148">スリー</span><span class="sxs-lookup"><span data-stu-id="afb6c-148">13</span></span>|<span data-ttu-id="afb6c-149">MFA チャレンジによるアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="afb6c-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="afb6c-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="afb6c-151">第</span><span class="sxs-lookup"><span data-stu-id="afb6c-151">14</span></span>|<span data-ttu-id="afb6c-152">AAD アクセスポリシーによって無効にされたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="afb6c-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="afb6c-153">compromisedPassword</span></span>|<span data-ttu-id="afb6c-154">約</span><span class="sxs-lookup"><span data-stu-id="afb6c-154">15</span></span>|<span data-ttu-id="afb6c-155">侵害されたパスワードによって取り消されたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="afb6c-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="afb6c-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="afb6c-157">16</span><span class="sxs-lookup"><span data-stu-id="afb6c-157">16</span></span>|<span data-ttu-id="afb6c-158">管理対象アプリケーションのチャレンジによって取り消されたアクセス状態</span><span class="sxs-lookup"><span data-stu-id="afb6c-158">Access state revoked by managed application challenge</span></span>|





