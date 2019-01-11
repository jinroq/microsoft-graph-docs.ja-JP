---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルの障害のカテゴリ。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd7ba949c95d507d956dd7f315b3c19e0759c20
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885527"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="06ce1-103">deviceEnrollmentFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="06ce1-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="06ce1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="06ce1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06ce1-105">登録の最上位レベルの障害のカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="06ce1-105">Top level failure categories for enrollment.</span></span>
## <a name="members"></a><span data-ttu-id="06ce1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="06ce1-106">Members</span></span>
|<span data-ttu-id="06ce1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="06ce1-107">Member</span></span>|<span data-ttu-id="06ce1-108">値</span><span class="sxs-lookup"><span data-stu-id="06ce1-108">Value</span></span>|<span data-ttu-id="06ce1-109">説明</span><span class="sxs-lookup"><span data-stu-id="06ce1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06ce1-110">不明</span><span class="sxs-lookup"><span data-stu-id="06ce1-110">unknown</span></span>|<span data-ttu-id="06ce1-111">0</span><span class="sxs-lookup"><span data-stu-id="06ce1-111">0</span></span>|<span data-ttu-id="06ce1-112">既定値、失敗の理由は不明です。</span><span class="sxs-lookup"><span data-stu-id="06ce1-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="06ce1-113">認証</span><span class="sxs-lookup"><span data-stu-id="06ce1-113">authentication</span></span>|<span data-ttu-id="06ce1-114">1</span><span class="sxs-lookup"><span data-stu-id="06ce1-114">1</span></span>|<span data-ttu-id="06ce1-115">認証に失敗しました</span><span class="sxs-lookup"><span data-stu-id="06ce1-115">Authentication failed</span></span>|
|<span data-ttu-id="06ce1-116">承認</span><span class="sxs-lookup"><span data-stu-id="06ce1-116">authorization</span></span>|<span data-ttu-id="06ce1-117">2</span><span class="sxs-lookup"><span data-stu-id="06ce1-117">2</span></span>|<span data-ttu-id="06ce1-118">呼び出しが認証されると、ですが、登録する権限がありませんでした。</span><span class="sxs-lookup"><span data-stu-id="06ce1-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="06ce1-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="06ce1-119">accountValidation</span></span>|<span data-ttu-id="06ce1-120">3</span><span class="sxs-lookup"><span data-stu-id="06ce1-120">3</span></span>|<span data-ttu-id="06ce1-121">登録用のアカウントを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="06ce1-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="06ce1-122">(アカウントがブロックされている登録が有効になっていません)</span><span class="sxs-lookup"><span data-stu-id="06ce1-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="06ce1-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="06ce1-123">userValidation</span></span>|<span data-ttu-id="06ce1-124">4</span><span class="sxs-lookup"><span data-stu-id="06ce1-124">4</span></span>|<span data-ttu-id="06ce1-125">ユーザーを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="06ce1-125">User could not be validated.</span></span> <span data-ttu-id="06ce1-126">(ユーザーが存在しない場合は、不足しているライセンス)</span><span class="sxs-lookup"><span data-stu-id="06ce1-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="06ce1-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="06ce1-127">deviceNotSupported</span></span>|<span data-ttu-id="06ce1-128">5</span><span class="sxs-lookup"><span data-stu-id="06ce1-128">5</span></span>|<span data-ttu-id="06ce1-129">モバイル デバイスの管理には、デバイスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06ce1-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="06ce1-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="06ce1-130">inMaintenance</span></span>|<span data-ttu-id="06ce1-131">6</span><span class="sxs-lookup"><span data-stu-id="06ce1-131">6</span></span>|<span data-ttu-id="06ce1-132">アカウントがメンテナンスします。</span><span class="sxs-lookup"><span data-stu-id="06ce1-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="06ce1-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="06ce1-133">badRequest</span></span>|<span data-ttu-id="06ce1-134">7</span><span class="sxs-lookup"><span data-stu-id="06ce1-134">7</span></span>|<span data-ttu-id="06ce1-135">サービスで認識されるサポートではない要求をクライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="06ce1-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="06ce1-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="06ce1-136">featureNotSupported</span></span>|<span data-ttu-id="06ce1-137">8</span><span class="sxs-lookup"><span data-stu-id="06ce1-137">8</span></span>|<span data-ttu-id="06ce1-138">このアカウントには、この登録で使用される機能はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06ce1-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="06ce1-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="06ce1-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="06ce1-140">9</span><span class="sxs-lookup"><span data-stu-id="06ce1-140">9</span></span>|<span data-ttu-id="06ce1-141">管理者によって構成されている登録の制限には、この登録がブロックされています。</span><span class="sxs-lookup"><span data-stu-id="06ce1-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="06ce1-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="06ce1-142">clientDisconnected</span></span>|<span data-ttu-id="06ce1-143">10</span><span class="sxs-lookup"><span data-stu-id="06ce1-143">10</span></span>|<span data-ttu-id="06ce1-144">クライアントがタイムアウトするか、登録は、エンド ・ ユーザーによって中止されました。</span><span class="sxs-lookup"><span data-stu-id="06ce1-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="06ce1-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="06ce1-145">userAbandonment</span></span>|<span data-ttu-id="06ce1-146">11</span><span class="sxs-lookup"><span data-stu-id="06ce1-146">11</span></span>|<span data-ttu-id="06ce1-147">登録は、エンド ・ ユーザーによって中断されました。</span><span class="sxs-lookup"><span data-stu-id="06ce1-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="06ce1-148">(エンド ・ ユーザーは、契約時の開始が、時間内に完了できませんでした)</span><span class="sxs-lookup"><span data-stu-id="06ce1-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
