---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 697dd182aa21d98418cfee056da8cc18b1aa0aee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967309"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="5608d-103">vppTokenActionFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="5608d-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="5608d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5608d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5608d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5608d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5608d-106">Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。</span><span class="sxs-lookup"><span data-stu-id="5608d-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="5608d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5608d-107">Members</span></span>
|<span data-ttu-id="5608d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5608d-108">Member</span></span>|<span data-ttu-id="5608d-109">値</span><span class="sxs-lookup"><span data-stu-id="5608d-109">Value</span></span>|<span data-ttu-id="5608d-110">説明</span><span class="sxs-lookup"><span data-stu-id="5608d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5608d-111">none</span><span class="sxs-lookup"><span data-stu-id="5608d-111">none</span></span>|<span data-ttu-id="5608d-112">.0</span><span class="sxs-lookup"><span data-stu-id="5608d-112">0</span></span>|<span data-ttu-id="5608d-113">なし</span><span class="sxs-lookup"><span data-stu-id="5608d-113">None.</span></span>|
|<span data-ttu-id="5608d-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="5608d-114">appleFailure</span></span>|<span data-ttu-id="5608d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5608d-115">1</span></span>|<span data-ttu-id="5608d-116">Apple のサービスでエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="5608d-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="5608d-117">internalError</span><span class="sxs-lookup"><span data-stu-id="5608d-117">internalError</span></span>|<span data-ttu-id="5608d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5608d-118">2</span></span>|<span data-ttu-id="5608d-119">内部エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="5608d-119">There was an internal error.</span></span>|
|<span data-ttu-id="5608d-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="5608d-120">expiredVppToken</span></span>|<span data-ttu-id="5608d-121">1/3</span><span class="sxs-lookup"><span data-stu-id="5608d-121">3</span></span>|<span data-ttu-id="5608d-122">Apple Volume Purchase Program のトークンの有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="5608d-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="5608d-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="5608d-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="5608d-124">2/4</span><span class="sxs-lookup"><span data-stu-id="5608d-124">4</span></span>|<span data-ttu-id="5608d-125">Apple Volume Purchase Program プッシュ通知証明書の有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="5608d-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





