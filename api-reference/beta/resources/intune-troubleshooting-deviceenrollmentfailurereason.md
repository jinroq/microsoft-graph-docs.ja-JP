---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルのエラーカテゴリ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae92cf0e9dc73dc2d846e549756fe1977fa19036
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951208"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="3b819-103">deviceEnrollmentFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="3b819-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="3b819-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b819-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b819-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3b819-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b819-106">登録の最上位レベルのエラーカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="3b819-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="3b819-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b819-107">Members</span></span>
|<span data-ttu-id="3b819-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b819-108">Member</span></span>|<span data-ttu-id="3b819-109">値</span><span class="sxs-lookup"><span data-stu-id="3b819-109">Value</span></span>|<span data-ttu-id="3b819-110">説明</span><span class="sxs-lookup"><span data-stu-id="3b819-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b819-111">不明</span><span class="sxs-lookup"><span data-stu-id="3b819-111">unknown</span></span>|<span data-ttu-id="3b819-112">.0</span><span class="sxs-lookup"><span data-stu-id="3b819-112">0</span></span>|<span data-ttu-id="3b819-113">既定値、エラーの理由は不明です。</span><span class="sxs-lookup"><span data-stu-id="3b819-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="3b819-114">認証</span><span class="sxs-lookup"><span data-stu-id="3b819-114">authentication</span></span>|<span data-ttu-id="3b819-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3b819-115">1</span></span>|<span data-ttu-id="3b819-116">認証に失敗した</span><span class="sxs-lookup"><span data-stu-id="3b819-116">Authentication failed</span></span>|
|<span data-ttu-id="3b819-117">手続き</span><span class="sxs-lookup"><span data-stu-id="3b819-117">authorization</span></span>|<span data-ttu-id="3b819-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3b819-118">2</span></span>|<span data-ttu-id="3b819-119">呼び出しは認証されましたが、登録が承認されていません。</span><span class="sxs-lookup"><span data-stu-id="3b819-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="3b819-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="3b819-120">accountValidation</span></span>|<span data-ttu-id="3b819-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3b819-121">3</span></span>|<span data-ttu-id="3b819-122">登録のためにアカウントを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="3b819-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="3b819-123">(アカウントがブロックされ、登録が有効になっていません)</span><span class="sxs-lookup"><span data-stu-id="3b819-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="3b819-124">userValidation</span><span class="sxs-lookup"><span data-stu-id="3b819-124">userValidation</span></span>|<span data-ttu-id="3b819-125">2/4</span><span class="sxs-lookup"><span data-stu-id="3b819-125">4</span></span>|<span data-ttu-id="3b819-126">ユーザーを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="3b819-126">User could not be validated.</span></span> <span data-ttu-id="3b819-127">(ユーザーが存在しません。ライセンスがありません)</span><span class="sxs-lookup"><span data-stu-id="3b819-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="3b819-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="3b819-128">deviceNotSupported</span></span>|<span data-ttu-id="3b819-129">5</span><span class="sxs-lookup"><span data-stu-id="3b819-129">5</span></span>|<span data-ttu-id="3b819-130">デバイスは、モバイルデバイス管理ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b819-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="3b819-131">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="3b819-131">inMaintenance</span></span>|<span data-ttu-id="3b819-132">シックス</span><span class="sxs-lookup"><span data-stu-id="3b819-132">6</span></span>|<span data-ttu-id="3b819-133">アカウントはメンテナンス中です。</span><span class="sxs-lookup"><span data-stu-id="3b819-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="3b819-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="3b819-134">badRequest</span></span>|<span data-ttu-id="3b819-135">7</span><span class="sxs-lookup"><span data-stu-id="3b819-135">7</span></span>|<span data-ttu-id="3b819-136">クライアントがサービスで認識/サポートされていない要求を送信しました。</span><span class="sxs-lookup"><span data-stu-id="3b819-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="3b819-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="3b819-137">featureNotSupported</span></span>|<span data-ttu-id="3b819-138">8 </span><span class="sxs-lookup"><span data-stu-id="3b819-138">8</span></span>|<span data-ttu-id="3b819-139">この登録で使用されている機能は、このアカウントではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b819-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="3b819-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="3b819-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="3b819-141">9 </span><span class="sxs-lookup"><span data-stu-id="3b819-141">9</span></span>|<span data-ttu-id="3b819-142">管理者によって構成された登録の制限は、この登録をブロックしました。</span><span class="sxs-lookup"><span data-stu-id="3b819-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="3b819-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="3b819-143">clientDisconnected</span></span>|<span data-ttu-id="3b819-144">10 </span><span class="sxs-lookup"><span data-stu-id="3b819-144">10</span></span>|<span data-ttu-id="3b819-145">クライアントがタイムアウトしたか、登録が enduser によって中止されました。</span><span class="sxs-lookup"><span data-stu-id="3b819-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="3b819-146">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="3b819-146">userAbandonment</span></span>|<span data-ttu-id="3b819-147">#</span><span class="sxs-lookup"><span data-stu-id="3b819-147">11</span></span>|<span data-ttu-id="3b819-148">登録は enduser によって中止されました。</span><span class="sxs-lookup"><span data-stu-id="3b819-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="3b819-149">(Enduser が開始されましたが、適切なタイミングで完了できませんでした)</span><span class="sxs-lookup"><span data-stu-id="3b819-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|




