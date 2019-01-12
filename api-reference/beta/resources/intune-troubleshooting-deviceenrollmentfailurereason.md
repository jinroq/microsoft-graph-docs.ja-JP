---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルの障害のカテゴリ。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 25834f9c6e972a5a12d3e8d1e2a1283646483000
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981036"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="15880-103">deviceEnrollmentFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="15880-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="15880-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15880-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15880-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15880-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15880-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15880-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15880-107">登録の最上位レベルの障害のカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="15880-107">Top level failure categories for enrollment.</span></span>
## <a name="members"></a><span data-ttu-id="15880-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="15880-108">Members</span></span>
|<span data-ttu-id="15880-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="15880-109">Member</span></span>|<span data-ttu-id="15880-110">値</span><span class="sxs-lookup"><span data-stu-id="15880-110">Value</span></span>|<span data-ttu-id="15880-111">説明</span><span class="sxs-lookup"><span data-stu-id="15880-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15880-112">不明</span><span class="sxs-lookup"><span data-stu-id="15880-112">unknown</span></span>|<span data-ttu-id="15880-113">0</span><span class="sxs-lookup"><span data-stu-id="15880-113">0</span></span>|<span data-ttu-id="15880-114">既定値、失敗の理由は不明です。</span><span class="sxs-lookup"><span data-stu-id="15880-114">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="15880-115">認証</span><span class="sxs-lookup"><span data-stu-id="15880-115">authentication</span></span>|<span data-ttu-id="15880-116">1</span><span class="sxs-lookup"><span data-stu-id="15880-116">1</span></span>|<span data-ttu-id="15880-117">認証に失敗しました</span><span class="sxs-lookup"><span data-stu-id="15880-117">Authentication failed</span></span>|
|<span data-ttu-id="15880-118">承認</span><span class="sxs-lookup"><span data-stu-id="15880-118">authorization</span></span>|<span data-ttu-id="15880-119">2</span><span class="sxs-lookup"><span data-stu-id="15880-119">2</span></span>|<span data-ttu-id="15880-120">呼び出しが認証されると、ですが、登録する権限がありませんでした。</span><span class="sxs-lookup"><span data-stu-id="15880-120">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="15880-121">accountValidation</span><span class="sxs-lookup"><span data-stu-id="15880-121">accountValidation</span></span>|<span data-ttu-id="15880-122">3</span><span class="sxs-lookup"><span data-stu-id="15880-122">3</span></span>|<span data-ttu-id="15880-123">登録用のアカウントを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="15880-123">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="15880-124">(アカウントがブロックされている登録が有効になっていません)</span><span class="sxs-lookup"><span data-stu-id="15880-124">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="15880-125">userValidation</span><span class="sxs-lookup"><span data-stu-id="15880-125">userValidation</span></span>|<span data-ttu-id="15880-126">4</span><span class="sxs-lookup"><span data-stu-id="15880-126">4</span></span>|<span data-ttu-id="15880-127">ユーザーを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="15880-127">User could not be validated.</span></span> <span data-ttu-id="15880-128">(ユーザーが存在しない場合は、不足しているライセンス)</span><span class="sxs-lookup"><span data-stu-id="15880-128">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="15880-129">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="15880-129">deviceNotSupported</span></span>|<span data-ttu-id="15880-130">5</span><span class="sxs-lookup"><span data-stu-id="15880-130">5</span></span>|<span data-ttu-id="15880-131">モバイル デバイスの管理には、デバイスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15880-131">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="15880-132">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="15880-132">inMaintenance</span></span>|<span data-ttu-id="15880-133">6</span><span class="sxs-lookup"><span data-stu-id="15880-133">6</span></span>|<span data-ttu-id="15880-134">アカウントがメンテナンスします。</span><span class="sxs-lookup"><span data-stu-id="15880-134">Account is in maintenance.</span></span>|
|<span data-ttu-id="15880-135">badRequest</span><span class="sxs-lookup"><span data-stu-id="15880-135">badRequest</span></span>|<span data-ttu-id="15880-136">7</span><span class="sxs-lookup"><span data-stu-id="15880-136">7</span></span>|<span data-ttu-id="15880-137">サービスで認識されるサポートではない要求をクライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="15880-137">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="15880-138">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="15880-138">featureNotSupported</span></span>|<span data-ttu-id="15880-139">8</span><span class="sxs-lookup"><span data-stu-id="15880-139">8</span></span>|<span data-ttu-id="15880-140">このアカウントには、この登録で使用される機能はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15880-140">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="15880-141">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="15880-141">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="15880-142">9</span><span class="sxs-lookup"><span data-stu-id="15880-142">9</span></span>|<span data-ttu-id="15880-143">管理者によって構成されている登録の制限には、この登録がブロックされています。</span><span class="sxs-lookup"><span data-stu-id="15880-143">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="15880-144">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="15880-144">clientDisconnected</span></span>|<span data-ttu-id="15880-145">10</span><span class="sxs-lookup"><span data-stu-id="15880-145">10</span></span>|<span data-ttu-id="15880-146">クライアントがタイムアウトするか、登録は、エンド ・ ユーザーによって中止されました。</span><span class="sxs-lookup"><span data-stu-id="15880-146">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="15880-147">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="15880-147">userAbandonment</span></span>|<span data-ttu-id="15880-148">11</span><span class="sxs-lookup"><span data-stu-id="15880-148">11</span></span>|<span data-ttu-id="15880-149">登録は、エンド ・ ユーザーによって中断されました。</span><span class="sxs-lookup"><span data-stu-id="15880-149">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="15880-150">(エンド ・ ユーザーは、契約時の開始が、時間内に完了できませんでした)</span><span class="sxs-lookup"><span data-stu-id="15880-150">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|





