---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0f8aacb6fc6f95b8c8085a78ed2851b16622357
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990989"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="f51fd-103">vppTokenActionFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="f51fd-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="f51fd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f51fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f51fd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f51fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f51fd-106">Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。</span><span class="sxs-lookup"><span data-stu-id="f51fd-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="f51fd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f51fd-107">Members</span></span>
|<span data-ttu-id="f51fd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f51fd-108">Member</span></span>|<span data-ttu-id="f51fd-109">値</span><span class="sxs-lookup"><span data-stu-id="f51fd-109">Value</span></span>|<span data-ttu-id="f51fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="f51fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f51fd-111">none</span><span class="sxs-lookup"><span data-stu-id="f51fd-111">none</span></span>|<span data-ttu-id="f51fd-112">.0</span><span class="sxs-lookup"><span data-stu-id="f51fd-112">0</span></span>|<span data-ttu-id="f51fd-113">なし</span><span class="sxs-lookup"><span data-stu-id="f51fd-113">None.</span></span>|
|<span data-ttu-id="f51fd-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="f51fd-114">appleFailure</span></span>|<span data-ttu-id="f51fd-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f51fd-115">1</span></span>|<span data-ttu-id="f51fd-116">Apple のサービスでエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="f51fd-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="f51fd-117">internalError</span><span class="sxs-lookup"><span data-stu-id="f51fd-117">internalError</span></span>|<span data-ttu-id="f51fd-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f51fd-118">2</span></span>|<span data-ttu-id="f51fd-119">内部エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="f51fd-119">There was an internal error.</span></span>|
|<span data-ttu-id="f51fd-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="f51fd-120">expiredVppToken</span></span>|<span data-ttu-id="f51fd-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f51fd-121">3</span></span>|<span data-ttu-id="f51fd-122">Apple Volume Purchase Program のトークンの有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="f51fd-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="f51fd-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="f51fd-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="f51fd-124">2/4</span><span class="sxs-lookup"><span data-stu-id="f51fd-124">4</span></span>|<span data-ttu-id="f51fd-125">Apple Volume Purchase Program プッシュ通知証明書の有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="f51fd-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|





