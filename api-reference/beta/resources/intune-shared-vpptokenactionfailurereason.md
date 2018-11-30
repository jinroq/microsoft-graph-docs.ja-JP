---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。
ms.openlocfilehash: 0fece0417a5585540f15e3f8a8631fd30eaa414e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069083"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="0830c-103">vppTokenActionFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="0830c-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="0830c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0830c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0830c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0830c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0830c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0830c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0830c-107">Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。</span><span class="sxs-lookup"><span data-stu-id="0830c-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>
## <a name="members"></a><span data-ttu-id="0830c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0830c-108">Members</span></span>
|<span data-ttu-id="0830c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0830c-109">Member</span></span>|<span data-ttu-id="0830c-110">値</span><span class="sxs-lookup"><span data-stu-id="0830c-110">Value</span></span>|<span data-ttu-id="0830c-111">説明</span><span class="sxs-lookup"><span data-stu-id="0830c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0830c-112">none</span><span class="sxs-lookup"><span data-stu-id="0830c-112">none</span></span>|<span data-ttu-id="0830c-113">0</span><span class="sxs-lookup"><span data-stu-id="0830c-113">0</span></span>|<span data-ttu-id="0830c-114">なし</span><span class="sxs-lookup"><span data-stu-id="0830c-114">None.</span></span>|
|<span data-ttu-id="0830c-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="0830c-115">appleFailure</span></span>|<span data-ttu-id="0830c-116">1</span><span class="sxs-lookup"><span data-stu-id="0830c-116">1</span></span>|<span data-ttu-id="0830c-117">Apple のサービスでエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0830c-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="0830c-118">internalError</span><span class="sxs-lookup"><span data-stu-id="0830c-118">internalError</span></span>|<span data-ttu-id="0830c-119">2</span><span class="sxs-lookup"><span data-stu-id="0830c-119">2</span></span>|<span data-ttu-id="0830c-120">内部エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0830c-120">There was an internal error.</span></span>|
|<span data-ttu-id="0830c-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="0830c-121">expiredVppToken</span></span>|<span data-ttu-id="0830c-122">3</span><span class="sxs-lookup"><span data-stu-id="0830c-122">3</span></span>|<span data-ttu-id="0830c-123">Apple ボリューム購入プログラムのトークンの有効期限が切れていたためにエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0830c-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="0830c-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0830c-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="0830c-125">4</span><span class="sxs-lookup"><span data-stu-id="0830c-125">4</span></span>|<span data-ttu-id="0830c-126">Apple ボリューム購入プログラムをプッシュ通知証明書の有効期限が切れているためにエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0830c-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





