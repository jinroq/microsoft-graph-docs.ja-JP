---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルのエラーカテゴリ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f03ce73f1d6f8b5edc6b3e3b661f9a7ba79407bb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163855"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="f8d00-103">deviceEnrollmentFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="f8d00-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="f8d00-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8d00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8d00-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f8d00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8d00-106">登録の最上位レベルのエラーカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="f8d00-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="f8d00-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8d00-107">Members</span></span>
|<span data-ttu-id="f8d00-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8d00-108">Member</span></span>|<span data-ttu-id="f8d00-109">値</span><span class="sxs-lookup"><span data-stu-id="f8d00-109">Value</span></span>|<span data-ttu-id="f8d00-110">説明</span><span class="sxs-lookup"><span data-stu-id="f8d00-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8d00-111">不明</span><span class="sxs-lookup"><span data-stu-id="f8d00-111">unknown</span></span>|<span data-ttu-id="f8d00-112">.0</span><span class="sxs-lookup"><span data-stu-id="f8d00-112">0</span></span>|<span data-ttu-id="f8d00-113">既定値、エラーの理由は不明です。</span><span class="sxs-lookup"><span data-stu-id="f8d00-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="f8d00-114">認証</span><span class="sxs-lookup"><span data-stu-id="f8d00-114">authentication</span></span>|<span data-ttu-id="f8d00-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f8d00-115">1</span></span>|<span data-ttu-id="f8d00-116">認証に失敗した</span><span class="sxs-lookup"><span data-stu-id="f8d00-116">Authentication failed</span></span>|
|<span data-ttu-id="f8d00-117">承認</span><span class="sxs-lookup"><span data-stu-id="f8d00-117">authorization</span></span>|<span data-ttu-id="f8d00-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f8d00-118">2</span></span>|<span data-ttu-id="f8d00-119">呼び出しは認証されましたが、登録が承認されていません。</span><span class="sxs-lookup"><span data-stu-id="f8d00-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="f8d00-120">accountvalidation</span><span class="sxs-lookup"><span data-stu-id="f8d00-120">accountValidation</span></span>|<span data-ttu-id="f8d00-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f8d00-121">3</span></span>|<span data-ttu-id="f8d00-122">登録のためにアカウントを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="f8d00-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="f8d00-123">(アカウントがブロックされ、登録が有効になっていません)</span><span class="sxs-lookup"><span data-stu-id="f8d00-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="f8d00-124">uservalidation</span><span class="sxs-lookup"><span data-stu-id="f8d00-124">userValidation</span></span>|<span data-ttu-id="f8d00-125">2/4</span><span class="sxs-lookup"><span data-stu-id="f8d00-125">4</span></span>|<span data-ttu-id="f8d00-126">ユーザーを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="f8d00-126">User could not be validated.</span></span> <span data-ttu-id="f8d00-127">(ユーザーが存在しません。ライセンスがありません)</span><span class="sxs-lookup"><span data-stu-id="f8d00-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="f8d00-128">devicenotsupported</span><span class="sxs-lookup"><span data-stu-id="f8d00-128">deviceNotSupported</span></span>|<span data-ttu-id="f8d00-129">5</span><span class="sxs-lookup"><span data-stu-id="f8d00-129">5</span></span>|<span data-ttu-id="f8d00-130">デバイスは、モバイルデバイス管理ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8d00-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="f8d00-131">inmaintenance</span><span class="sxs-lookup"><span data-stu-id="f8d00-131">inMaintenance</span></span>|<span data-ttu-id="f8d00-132">シックス</span><span class="sxs-lookup"><span data-stu-id="f8d00-132">6</span></span>|<span data-ttu-id="f8d00-133">アカウントはメンテナンス中です。</span><span class="sxs-lookup"><span data-stu-id="f8d00-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="f8d00-134">badrequest</span><span class="sxs-lookup"><span data-stu-id="f8d00-134">badRequest</span></span>|<span data-ttu-id="f8d00-135">7</span><span class="sxs-lookup"><span data-stu-id="f8d00-135">7</span></span>|<span data-ttu-id="f8d00-136">クライアントがサービスで認識/サポートされていない要求を送信しました。</span><span class="sxs-lookup"><span data-stu-id="f8d00-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="f8d00-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="f8d00-137">featureNotSupported</span></span>|<span data-ttu-id="f8d00-138">~</span><span class="sxs-lookup"><span data-stu-id="f8d00-138">8</span></span>|<span data-ttu-id="f8d00-139">この登録で使用されている機能は、このアカウントではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8d00-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="f8d00-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="f8d00-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="f8d00-141">i-9</span><span class="sxs-lookup"><span data-stu-id="f8d00-141">9</span></span>|<span data-ttu-id="f8d00-142">管理者によって構成された登録の制限は、この登録をブロックしました。</span><span class="sxs-lookup"><span data-stu-id="f8d00-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="f8d00-143">clientdisconnected</span><span class="sxs-lookup"><span data-stu-id="f8d00-143">clientDisconnected</span></span>|<span data-ttu-id="f8d00-144">個</span><span class="sxs-lookup"><span data-stu-id="f8d00-144">10</span></span>|<span data-ttu-id="f8d00-145">クライアントがタイムアウトしたか、登録が enduser によって中止されました。</span><span class="sxs-lookup"><span data-stu-id="f8d00-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="f8d00-146">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="f8d00-146">userAbandonment</span></span>|<span data-ttu-id="f8d00-147">#</span><span class="sxs-lookup"><span data-stu-id="f8d00-147">11</span></span>|<span data-ttu-id="f8d00-148">登録は enduser によって中止されました。</span><span class="sxs-lookup"><span data-stu-id="f8d00-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="f8d00-149">(Enduser が開始されましたが、適切なタイミングで完了できませんでした)</span><span class="sxs-lookup"><span data-stu-id="f8d00-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|




