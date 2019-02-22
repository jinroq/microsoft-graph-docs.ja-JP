---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05d3137bb5aac2aef3024825df5e7e0b84ffde51
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169693"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="36f37-103">vppTokenActionFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="36f37-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="36f37-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36f37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36f37-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36f37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36f37-106">Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。</span><span class="sxs-lookup"><span data-stu-id="36f37-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="36f37-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="36f37-107">Members</span></span>
|<span data-ttu-id="36f37-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="36f37-108">Member</span></span>|<span data-ttu-id="36f37-109">値</span><span class="sxs-lookup"><span data-stu-id="36f37-109">Value</span></span>|<span data-ttu-id="36f37-110">説明</span><span class="sxs-lookup"><span data-stu-id="36f37-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36f37-111">none</span><span class="sxs-lookup"><span data-stu-id="36f37-111">none</span></span>|<span data-ttu-id="36f37-112">.0</span><span class="sxs-lookup"><span data-stu-id="36f37-112">0</span></span>|<span data-ttu-id="36f37-113">なし</span><span class="sxs-lookup"><span data-stu-id="36f37-113">None.</span></span>|
|<span data-ttu-id="36f37-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="36f37-114">appleFailure</span></span>|<span data-ttu-id="36f37-115">1-d</span><span class="sxs-lookup"><span data-stu-id="36f37-115">1</span></span>|<span data-ttu-id="36f37-116">Apple のサービスでエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="36f37-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="36f37-117">internalError</span><span class="sxs-lookup"><span data-stu-id="36f37-117">internalError</span></span>|<span data-ttu-id="36f37-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="36f37-118">2</span></span>|<span data-ttu-id="36f37-119">内部エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="36f37-119">There was an internal error.</span></span>|
|<span data-ttu-id="36f37-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="36f37-120">expiredVppToken</span></span>|<span data-ttu-id="36f37-121">1/3</span><span class="sxs-lookup"><span data-stu-id="36f37-121">3</span></span>|<span data-ttu-id="36f37-122">Apple volume purchase program のトークンの有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="36f37-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="36f37-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="36f37-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="36f37-124">2/4</span><span class="sxs-lookup"><span data-stu-id="36f37-124">4</span></span>|<span data-ttu-id="36f37-125">Apple volume purchase program プッシュ通知証明書の有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="36f37-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|




