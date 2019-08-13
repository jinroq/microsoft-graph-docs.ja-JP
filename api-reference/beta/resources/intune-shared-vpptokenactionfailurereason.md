---
title: vppTokenActionFailureReason 列挙型
description: Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 144572ab0d18949ace682681a4939ca17a4538a2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347844"
---
# <a name="vpptokenactionfailurereason-enum-type"></a><span data-ttu-id="0bb13-103">vppTokenActionFailureReason 列挙型</span><span class="sxs-lookup"><span data-stu-id="0bb13-103">vppTokenActionFailureReason enum type</span></span>

> <span data-ttu-id="0bb13-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bb13-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bb13-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0bb13-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bb13-106">Apple ボリューム購入プログラムのトークンアクションが失敗した場合に考えられる理由の種類。</span><span class="sxs-lookup"><span data-stu-id="0bb13-106">Possible types of reasons for an Apple Volume Purchase Program token action failure.</span></span>

## <a name="members"></a><span data-ttu-id="0bb13-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0bb13-107">Members</span></span>
|<span data-ttu-id="0bb13-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0bb13-108">Member</span></span>|<span data-ttu-id="0bb13-109">値</span><span class="sxs-lookup"><span data-stu-id="0bb13-109">Value</span></span>|<span data-ttu-id="0bb13-110">説明</span><span class="sxs-lookup"><span data-stu-id="0bb13-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bb13-111">none</span><span class="sxs-lookup"><span data-stu-id="0bb13-111">none</span></span>|<span data-ttu-id="0bb13-112">.0</span><span class="sxs-lookup"><span data-stu-id="0bb13-112">0</span></span>|<span data-ttu-id="0bb13-113">なし</span><span class="sxs-lookup"><span data-stu-id="0bb13-113">None.</span></span>|
|<span data-ttu-id="0bb13-114">appleFailure</span><span class="sxs-lookup"><span data-stu-id="0bb13-114">appleFailure</span></span>|<span data-ttu-id="0bb13-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0bb13-115">1</span></span>|<span data-ttu-id="0bb13-116">Apple のサービスでエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0bb13-116">There was an error on Apple's service.</span></span>|
|<span data-ttu-id="0bb13-117">internalError</span><span class="sxs-lookup"><span data-stu-id="0bb13-117">internalError</span></span>|<span data-ttu-id="0bb13-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0bb13-118">2</span></span>|<span data-ttu-id="0bb13-119">内部エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0bb13-119">There was an internal error.</span></span>|
|<span data-ttu-id="0bb13-120">expiredVppToken</span><span class="sxs-lookup"><span data-stu-id="0bb13-120">expiredVppToken</span></span>|<span data-ttu-id="0bb13-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0bb13-121">3</span></span>|<span data-ttu-id="0bb13-122">Apple Volume Purchase Program のトークンの有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0bb13-122">There was an error because the Apple Volume Purchase Program token was expired.</span></span>|
|<span data-ttu-id="0bb13-123">expiredApplePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0bb13-123">expiredApplePushNotificationCertificate</span></span>|<span data-ttu-id="0bb13-124">2/4</span><span class="sxs-lookup"><span data-stu-id="0bb13-124">4</span></span>|<span data-ttu-id="0bb13-125">Apple Volume Purchase Program プッシュ通知証明書の有効期限が切れたため、エラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0bb13-125">There was an error because the Apple Volume Purchase Program Push Notification certificate expired.</span></span>|



