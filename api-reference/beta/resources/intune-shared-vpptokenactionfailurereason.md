---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba4c339b774fd32a852925729e2e158dc13e52d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393145"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="cc8ed-103">vppTokenActionFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="cc8ed-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="cc8ed-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc8ed-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc8ed-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc8ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc8ed-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc8ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc8ed-107">Apple ボリューム購入プログラム トークンの操作エラーが発生する理由の種類です。</span><span class="sxs-lookup"><span data-stu-id="cc8ed-107">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="cc8ed-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="cc8ed-108">Members</span></span>
|<span data-ttu-id="cc8ed-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="cc8ed-109">Member</span></span>|<span data-ttu-id="cc8ed-110">値</span><span class="sxs-lookup"><span data-stu-id="cc8ed-110">Value</span></span>|<span data-ttu-id="cc8ed-111">説明</span><span class="sxs-lookup"><span data-stu-id="cc8ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc8ed-112">none</span><span class="sxs-lookup"><span data-stu-id="cc8ed-112">none</span></span>|<span data-ttu-id="cc8ed-113">0</span><span class="sxs-lookup"><span data-stu-id="cc8ed-113">0</span></span>|<span data-ttu-id="cc8ed-114">なし</span><span class="sxs-lookup"><span data-stu-id="cc8ed-114">None.</span></span>|
|<span data-ttu-id="cc8ed-115">appleFailure</span><span class="sxs-lookup"><span data-stu-id="cc8ed-115">appleFailure</span></span>|<span data-ttu-id="cc8ed-116">1</span><span class="sxs-lookup"><span data-stu-id="cc8ed-116">1</span></span>|<span data-ttu-id="cc8ed-117">Apple のサービスでエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="cc8ed-117">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="cc8ed-118">internalError</span><span class="sxs-lookup"><span data-stu-id="cc8ed-118">internalError</span></span>|<span data-ttu-id="cc8ed-119">2</span><span class="sxs-lookup"><span data-stu-id="cc8ed-119">2</span></span>|<span data-ttu-id="cc8ed-120">内部エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="cc8ed-120">There was an internal error.</span></span>|
|<span data-ttu-id="cc8ed-121">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="cc8ed-121">expiredVppToken</span></span>|<span data-ttu-id="cc8ed-122">3</span><span class="sxs-lookup"><span data-stu-id="cc8ed-122">3</span></span>|<span data-ttu-id="cc8ed-123">Apple ボリューム購入プログラムのトークンの有効期限が切れていたためにエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="cc8ed-123">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="cc8ed-124">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="cc8ed-124">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="cc8ed-125">4</span><span class="sxs-lookup"><span data-stu-id="cc8ed-125">4</span></span>|<span data-ttu-id="cc8ed-126">Apple ボリューム購入プログラムをプッシュ通知証明書の有効期限が切れているためにエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="cc8ed-126">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




