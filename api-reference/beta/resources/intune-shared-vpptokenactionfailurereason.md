---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9adb896d384be99496c016ef3bd39b02ff1a28e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548258"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="6a63d-103">vppTokenActionFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="6a63d-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="6a63d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a63d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a63d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a63d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a63d-106">Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。</span><span class="sxs-lookup"><span data-stu-id="6a63d-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="6a63d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6a63d-107">Members</span></span>
|<span data-ttu-id="6a63d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6a63d-108">Member</span></span>|<span data-ttu-id="6a63d-109">値</span><span class="sxs-lookup"><span data-stu-id="6a63d-109">Value</span></span>|<span data-ttu-id="6a63d-110">説明</span><span class="sxs-lookup"><span data-stu-id="6a63d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a63d-111">なし</span><span class="sxs-lookup"><span data-stu-id="6a63d-111">none</span></span>|<span data-ttu-id="6a63d-112">.0</span><span class="sxs-lookup"><span data-stu-id="6a63d-112">0</span></span>|<span data-ttu-id="6a63d-113">なし</span><span class="sxs-lookup"><span data-stu-id="6a63d-113">None.</span></span>|
|<span data-ttu-id="6a63d-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="6a63d-114">appleFailure</span></span>|<span data-ttu-id="6a63d-115">1 </span><span class="sxs-lookup"><span data-stu-id="6a63d-115">1</span></span>|<span data-ttu-id="6a63d-116">Apple のサービスでエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="6a63d-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="6a63d-117">internalError</span><span class="sxs-lookup"><span data-stu-id="6a63d-117">internalError</span></span>|<span data-ttu-id="6a63d-118">2 </span><span class="sxs-lookup"><span data-stu-id="6a63d-118">2</span></span>|<span data-ttu-id="6a63d-119">内部エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="6a63d-119">There was an internal error.</span></span>|
|<span data-ttu-id="6a63d-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="6a63d-120">expiredVppToken</span></span>|<span data-ttu-id="6a63d-121">3 </span><span class="sxs-lookup"><span data-stu-id="6a63d-121">3</span></span>|<span data-ttu-id="6a63d-122">Apple volume purchase program のトークンの有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="6a63d-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="6a63d-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="6a63d-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="6a63d-124">4 </span><span class="sxs-lookup"><span data-stu-id="6a63d-124">4</span></span>|<span data-ttu-id="6a63d-125">Apple volume purchase program プッシュ通知証明書の有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="6a63d-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





