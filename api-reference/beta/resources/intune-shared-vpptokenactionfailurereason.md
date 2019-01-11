---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f488302b7fc701e8a419357ad7d6cbbb6015759b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883721"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="da96b-103">vppTokenActionFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="da96b-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="da96b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da96b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da96b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da96b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da96b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="da96b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da96b-107">Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。</span><span class="sxs-lookup"><span data-stu-id="da96b-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="da96b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="da96b-108">Members</span></span>
|<span data-ttu-id="da96b-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="da96b-109">Member</span></span>|<span data-ttu-id="da96b-110">値</span><span class="sxs-lookup"><span data-stu-id="da96b-110">Value</span></span>|<span data-ttu-id="da96b-111">説明</span><span class="sxs-lookup"><span data-stu-id="da96b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da96b-112">none</span><span class="sxs-lookup"><span data-stu-id="da96b-112">none</span></span>|<span data-ttu-id="da96b-113">0</span><span class="sxs-lookup"><span data-stu-id="da96b-113">0</span></span>|<span data-ttu-id="da96b-114">なし</span><span class="sxs-lookup"><span data-stu-id="da96b-114">None.</span></span>|
|<span data-ttu-id="da96b-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="da96b-115">appleFailure</span></span>|<span data-ttu-id="da96b-116">1</span><span class="sxs-lookup"><span data-stu-id="da96b-116">1</span></span>|<span data-ttu-id="da96b-117">Apple のサービスでエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="da96b-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="da96b-118">internalError</span><span class="sxs-lookup"><span data-stu-id="da96b-118">internalError</span></span>|<span data-ttu-id="da96b-119">2</span><span class="sxs-lookup"><span data-stu-id="da96b-119">2</span></span>|<span data-ttu-id="da96b-120">内部エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="da96b-120">There was an internal error.</span></span>|
|<span data-ttu-id="da96b-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="da96b-121">expiredVppToken</span></span>|<span data-ttu-id="da96b-122">3</span><span class="sxs-lookup"><span data-stu-id="da96b-122">3</span></span>|<span data-ttu-id="da96b-123">Apple ボリューム購入プログラムのトークンの有効期限が切れていたためにエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="da96b-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="da96b-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="da96b-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="da96b-125">4</span><span class="sxs-lookup"><span data-stu-id="da96b-125">4</span></span>|<span data-ttu-id="da96b-126">Apple ボリューム購入プログラムをプッシュ通知証明書の有効期限が切れているためにエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="da96b-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





