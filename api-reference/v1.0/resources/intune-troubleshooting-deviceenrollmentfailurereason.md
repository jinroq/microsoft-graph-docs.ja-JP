---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルの障害のカテゴリ。
author: tfitzmac
ms.openlocfilehash: 6adf8918762832dd961a7cd3f2b625f2394c54cb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343954"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="0ca58-103">deviceEnrollmentFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="0ca58-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="0ca58-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ca58-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ca58-105">登録の最上位レベルの障害のカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="0ca58-105">Top level failure categories for enrollment.</span></span>
## <a name="members"></a><span data-ttu-id="0ca58-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0ca58-106">Members</span></span>
|<span data-ttu-id="0ca58-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0ca58-107">Member</span></span>|<span data-ttu-id="0ca58-108">値</span><span class="sxs-lookup"><span data-stu-id="0ca58-108">Value</span></span>|<span data-ttu-id="0ca58-109">説明</span><span class="sxs-lookup"><span data-stu-id="0ca58-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ca58-110">不明</span><span class="sxs-lookup"><span data-stu-id="0ca58-110">unknown</span></span>|<span data-ttu-id="0ca58-111">0</span><span class="sxs-lookup"><span data-stu-id="0ca58-111">0</span></span>|<span data-ttu-id="0ca58-112">既定値、失敗の理由は不明です。</span><span class="sxs-lookup"><span data-stu-id="0ca58-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="0ca58-113">認証</span><span class="sxs-lookup"><span data-stu-id="0ca58-113">authentication</span></span>|<span data-ttu-id="0ca58-114">1</span><span class="sxs-lookup"><span data-stu-id="0ca58-114">1</span></span>|<span data-ttu-id="0ca58-115">認証に失敗しました</span><span class="sxs-lookup"><span data-stu-id="0ca58-115">Authentication failed</span></span>|
|<span data-ttu-id="0ca58-116">承認</span><span class="sxs-lookup"><span data-stu-id="0ca58-116">authorization</span></span>|<span data-ttu-id="0ca58-117">2</span><span class="sxs-lookup"><span data-stu-id="0ca58-117">2</span></span>|<span data-ttu-id="0ca58-118">呼び出しが認証されると、ですが、登録する権限がありませんでした。</span><span class="sxs-lookup"><span data-stu-id="0ca58-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="0ca58-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="0ca58-119">accountValidation</span></span>|<span data-ttu-id="0ca58-120">3</span><span class="sxs-lookup"><span data-stu-id="0ca58-120">3</span></span>|<span data-ttu-id="0ca58-121">登録用のアカウントを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0ca58-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="0ca58-122">(アカウントがブロックされている登録が有効になっていません)</span><span class="sxs-lookup"><span data-stu-id="0ca58-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="0ca58-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="0ca58-123">userValidation</span></span>|<span data-ttu-id="0ca58-124">4</span><span class="sxs-lookup"><span data-stu-id="0ca58-124">4</span></span>|<span data-ttu-id="0ca58-125">ユーザーを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0ca58-125">User could not be validated.</span></span> <span data-ttu-id="0ca58-126">(ユーザーが存在しない場合は、不足しているライセンス)</span><span class="sxs-lookup"><span data-stu-id="0ca58-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="0ca58-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="0ca58-127">deviceNotSupported</span></span>|<span data-ttu-id="0ca58-128">5</span><span class="sxs-lookup"><span data-stu-id="0ca58-128">5</span></span>|<span data-ttu-id="0ca58-129">モバイル デバイスの管理には、デバイスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ca58-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="0ca58-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="0ca58-130">inMaintenance</span></span>|<span data-ttu-id="0ca58-131">6</span><span class="sxs-lookup"><span data-stu-id="0ca58-131">6</span></span>|<span data-ttu-id="0ca58-132">アカウントがメンテナンスします。</span><span class="sxs-lookup"><span data-stu-id="0ca58-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="0ca58-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="0ca58-133">badRequest</span></span>|<span data-ttu-id="0ca58-134">7</span><span class="sxs-lookup"><span data-stu-id="0ca58-134">7</span></span>|<span data-ttu-id="0ca58-135">サービスで認識されるサポートではない要求をクライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="0ca58-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="0ca58-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="0ca58-136">featureNotSupported</span></span>|<span data-ttu-id="0ca58-137">8</span><span class="sxs-lookup"><span data-stu-id="0ca58-137">8</span></span>|<span data-ttu-id="0ca58-138">このアカウントには、この登録で使用される機能はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ca58-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="0ca58-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="0ca58-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="0ca58-140">9</span><span class="sxs-lookup"><span data-stu-id="0ca58-140">9</span></span>|<span data-ttu-id="0ca58-141">管理者によって構成されている登録の制限には、この登録がブロックされています。</span><span class="sxs-lookup"><span data-stu-id="0ca58-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="0ca58-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="0ca58-142">clientDisconnected</span></span>|<span data-ttu-id="0ca58-143">10</span><span class="sxs-lookup"><span data-stu-id="0ca58-143">10</span></span>|<span data-ttu-id="0ca58-144">クライアントがタイムアウトするか、登録は、エンド ・ ユーザーによって中止されました。</span><span class="sxs-lookup"><span data-stu-id="0ca58-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="0ca58-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="0ca58-145">userAbandonment</span></span>|<span data-ttu-id="0ca58-146">11</span><span class="sxs-lookup"><span data-stu-id="0ca58-146">11</span></span>|<span data-ttu-id="0ca58-147">登録は、エンド ・ ユーザーによって中断されました。</span><span class="sxs-lookup"><span data-stu-id="0ca58-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="0ca58-148">(エンド ・ ユーザーは、契約時の開始が、時間内に完了できませんでした)</span><span class="sxs-lookup"><span data-stu-id="0ca58-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
