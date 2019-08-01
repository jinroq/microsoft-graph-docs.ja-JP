---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルのエラーカテゴリ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 742c30da453a8de814dad0a70fae2be2946f1127
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036793"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="02c6d-103">deviceEnrollmentFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="02c6d-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="02c6d-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="02c6d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02c6d-105">登録の最上位レベルのエラーカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="02c6d-105">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="02c6d-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="02c6d-106">Members</span></span>
|<span data-ttu-id="02c6d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="02c6d-107">Member</span></span>|<span data-ttu-id="02c6d-108">値</span><span class="sxs-lookup"><span data-stu-id="02c6d-108">Value</span></span>|<span data-ttu-id="02c6d-109">説明</span><span class="sxs-lookup"><span data-stu-id="02c6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02c6d-110">不明</span><span class="sxs-lookup"><span data-stu-id="02c6d-110">unknown</span></span>|<span data-ttu-id="02c6d-111">.0</span><span class="sxs-lookup"><span data-stu-id="02c6d-111">0</span></span>|<span data-ttu-id="02c6d-112">既定値、エラーの理由は不明です。</span><span class="sxs-lookup"><span data-stu-id="02c6d-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="02c6d-113">認証</span><span class="sxs-lookup"><span data-stu-id="02c6d-113">authentication</span></span>|<span data-ttu-id="02c6d-114">1-d</span><span class="sxs-lookup"><span data-stu-id="02c6d-114">1</span></span>|<span data-ttu-id="02c6d-115">認証に失敗した</span><span class="sxs-lookup"><span data-stu-id="02c6d-115">Authentication failed</span></span>|
|<span data-ttu-id="02c6d-116">手続き</span><span class="sxs-lookup"><span data-stu-id="02c6d-116">authorization</span></span>|<span data-ttu-id="02c6d-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="02c6d-117">2</span></span>|<span data-ttu-id="02c6d-118">呼び出しは認証されましたが、登録が承認されていません。</span><span class="sxs-lookup"><span data-stu-id="02c6d-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="02c6d-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="02c6d-119">accountValidation</span></span>|<span data-ttu-id="02c6d-120">1/3</span><span class="sxs-lookup"><span data-stu-id="02c6d-120">3</span></span>|<span data-ttu-id="02c6d-121">登録のためにアカウントを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="02c6d-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="02c6d-122">(アカウントがブロックされ、登録が有効になっていません)</span><span class="sxs-lookup"><span data-stu-id="02c6d-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="02c6d-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="02c6d-123">userValidation</span></span>|<span data-ttu-id="02c6d-124">2/4</span><span class="sxs-lookup"><span data-stu-id="02c6d-124">4</span></span>|<span data-ttu-id="02c6d-125">ユーザーを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="02c6d-125">User could not be validated.</span></span> <span data-ttu-id="02c6d-126">(ユーザーが存在しません。ライセンスがありません)</span><span class="sxs-lookup"><span data-stu-id="02c6d-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="02c6d-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="02c6d-127">deviceNotSupported</span></span>|<span data-ttu-id="02c6d-128">5</span><span class="sxs-lookup"><span data-stu-id="02c6d-128">5</span></span>|<span data-ttu-id="02c6d-129">デバイスは、モバイルデバイス管理ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02c6d-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="02c6d-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="02c6d-130">inMaintenance</span></span>|<span data-ttu-id="02c6d-131">シックス</span><span class="sxs-lookup"><span data-stu-id="02c6d-131">6</span></span>|<span data-ttu-id="02c6d-132">アカウントはメンテナンス中です。</span><span class="sxs-lookup"><span data-stu-id="02c6d-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="02c6d-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="02c6d-133">badRequest</span></span>|<span data-ttu-id="02c6d-134">7</span><span class="sxs-lookup"><span data-stu-id="02c6d-134">7</span></span>|<span data-ttu-id="02c6d-135">クライアントがサービスで認識/サポートされていない要求を送信しました。</span><span class="sxs-lookup"><span data-stu-id="02c6d-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="02c6d-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="02c6d-136">featureNotSupported</span></span>|<span data-ttu-id="02c6d-137">8 </span><span class="sxs-lookup"><span data-stu-id="02c6d-137">8</span></span>|<span data-ttu-id="02c6d-138">この登録で使用されている機能は、このアカウントではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02c6d-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="02c6d-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="02c6d-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="02c6d-140">9 </span><span class="sxs-lookup"><span data-stu-id="02c6d-140">9</span></span>|<span data-ttu-id="02c6d-141">管理者によって構成された登録の制限は、この登録をブロックしました。</span><span class="sxs-lookup"><span data-stu-id="02c6d-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="02c6d-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="02c6d-142">clientDisconnected</span></span>|<span data-ttu-id="02c6d-143">10 </span><span class="sxs-lookup"><span data-stu-id="02c6d-143">10</span></span>|<span data-ttu-id="02c6d-144">クライアントがタイムアウトしたか、登録が enduser によって中止されました。</span><span class="sxs-lookup"><span data-stu-id="02c6d-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="02c6d-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="02c6d-145">userAbandonment</span></span>|<span data-ttu-id="02c6d-146">#</span><span class="sxs-lookup"><span data-stu-id="02c6d-146">11</span></span>|<span data-ttu-id="02c6d-147">登録は enduser によって中止されました。</span><span class="sxs-lookup"><span data-stu-id="02c6d-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="02c6d-148">(Enduser が開始されましたが、適切なタイミングで完了できませんでした)</span><span class="sxs-lookup"><span data-stu-id="02c6d-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

