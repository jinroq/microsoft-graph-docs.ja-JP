---
title: deviceEnrollmentFailureReason 列挙型
description: 登録の最上位レベルの障害のカテゴリ。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fbfe7193c72f1ff1a03a7e7bb4da57d0a032e530
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396211"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="38be1-103">deviceEnrollmentFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="38be1-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="38be1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="38be1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38be1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38be1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38be1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="38be1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38be1-107">登録の最上位レベルの障害のカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="38be1-107">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="38be1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="38be1-108">Members</span></span>
|<span data-ttu-id="38be1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="38be1-109">Member</span></span>|<span data-ttu-id="38be1-110">値</span><span class="sxs-lookup"><span data-stu-id="38be1-110">Value</span></span>|<span data-ttu-id="38be1-111">説明</span><span class="sxs-lookup"><span data-stu-id="38be1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38be1-112">不明</span><span class="sxs-lookup"><span data-stu-id="38be1-112">unknown</span></span>|<span data-ttu-id="38be1-113">0</span><span class="sxs-lookup"><span data-stu-id="38be1-113">0</span></span>|<span data-ttu-id="38be1-114">既定値、失敗の理由は不明です。</span><span class="sxs-lookup"><span data-stu-id="38be1-114">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="38be1-115">認証</span><span class="sxs-lookup"><span data-stu-id="38be1-115">authentication</span></span>|<span data-ttu-id="38be1-116">1</span><span class="sxs-lookup"><span data-stu-id="38be1-116">1</span></span>|<span data-ttu-id="38be1-117">認証に失敗しました</span><span class="sxs-lookup"><span data-stu-id="38be1-117">Authentication failed</span></span>|
|<span data-ttu-id="38be1-118">承認</span><span class="sxs-lookup"><span data-stu-id="38be1-118">authorization</span></span>|<span data-ttu-id="38be1-119">2</span><span class="sxs-lookup"><span data-stu-id="38be1-119">2</span></span>|<span data-ttu-id="38be1-120">呼び出しが認証されると、ですが、登録する権限がありませんでした。</span><span class="sxs-lookup"><span data-stu-id="38be1-120">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="38be1-121">accountValidation</span><span class="sxs-lookup"><span data-stu-id="38be1-121">accountValidation</span></span>|<span data-ttu-id="38be1-122">3</span><span class="sxs-lookup"><span data-stu-id="38be1-122">3</span></span>|<span data-ttu-id="38be1-123">登録用のアカウントを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="38be1-123">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="38be1-124">(アカウントがブロックされている登録が有効になっていません)</span><span class="sxs-lookup"><span data-stu-id="38be1-124">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="38be1-125">userValidation</span><span class="sxs-lookup"><span data-stu-id="38be1-125">userValidation</span></span>|<span data-ttu-id="38be1-126">4</span><span class="sxs-lookup"><span data-stu-id="38be1-126">4</span></span>|<span data-ttu-id="38be1-127">ユーザーを検証できませんでした。</span><span class="sxs-lookup"><span data-stu-id="38be1-127">User could not be validated.</span></span> <span data-ttu-id="38be1-128">(ユーザーが存在しない場合は、不足しているライセンス)</span><span class="sxs-lookup"><span data-stu-id="38be1-128">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="38be1-129">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="38be1-129">deviceNotSupported</span></span>|<span data-ttu-id="38be1-130">5</span><span class="sxs-lookup"><span data-stu-id="38be1-130">5</span></span>|<span data-ttu-id="38be1-131">モバイル デバイスの管理には、デバイスはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38be1-131">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="38be1-132">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="38be1-132">inMaintenance</span></span>|<span data-ttu-id="38be1-133">6</span><span class="sxs-lookup"><span data-stu-id="38be1-133">6</span></span>|<span data-ttu-id="38be1-134">アカウントがメンテナンスします。</span><span class="sxs-lookup"><span data-stu-id="38be1-134">Account is in maintenance.</span></span>|
|<span data-ttu-id="38be1-135">badRequest</span><span class="sxs-lookup"><span data-stu-id="38be1-135">badRequest</span></span>|<span data-ttu-id="38be1-136">7</span><span class="sxs-lookup"><span data-stu-id="38be1-136">7</span></span>|<span data-ttu-id="38be1-137">サービスで認識されるサポートではない要求をクライアントに送信されます。</span><span class="sxs-lookup"><span data-stu-id="38be1-137">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="38be1-138">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="38be1-138">featureNotSupported</span></span>|<span data-ttu-id="38be1-139">8</span><span class="sxs-lookup"><span data-stu-id="38be1-139">8</span></span>|<span data-ttu-id="38be1-140">このアカウントには、この登録で使用される機能はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38be1-140">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="38be1-141">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="38be1-141">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="38be1-142">9</span><span class="sxs-lookup"><span data-stu-id="38be1-142">9</span></span>|<span data-ttu-id="38be1-143">管理者によって構成されている登録の制限には、この登録がブロックされています。</span><span class="sxs-lookup"><span data-stu-id="38be1-143">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="38be1-144">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="38be1-144">clientDisconnected</span></span>|<span data-ttu-id="38be1-145">10</span><span class="sxs-lookup"><span data-stu-id="38be1-145">10</span></span>|<span data-ttu-id="38be1-146">クライアントがタイムアウトするか、登録は、エンド ・ ユーザーによって中止されました。</span><span class="sxs-lookup"><span data-stu-id="38be1-146">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="38be1-147">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="38be1-147">userAbandonment</span></span>|<span data-ttu-id="38be1-148">11</span><span class="sxs-lookup"><span data-stu-id="38be1-148">11</span></span>|<span data-ttu-id="38be1-149">登録は、エンド ・ ユーザーによって中断されました。</span><span class="sxs-lookup"><span data-stu-id="38be1-149">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="38be1-150">(エンド ・ ユーザーは、契約時の開始が、時間内に完了できませんでした)</span><span class="sxs-lookup"><span data-stu-id="38be1-150">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|




