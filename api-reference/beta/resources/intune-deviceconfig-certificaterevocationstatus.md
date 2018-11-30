---
title: certificateRevocationStatus 列挙型
description: 証明書失効の状態です。
ms.openlocfilehash: 5fb80b85cb6fe65e20439f8a3242b6bc74b30184
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067940"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="ae2e7-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="ae2e7-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="ae2e7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae2e7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae2e7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae2e7-107">証明書失効の状態です。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="ae2e7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae2e7-108">Members</span></span>
|<span data-ttu-id="ae2e7-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ae2e7-109">Member</span></span>|<span data-ttu-id="ae2e7-110">値</span><span class="sxs-lookup"><span data-stu-id="ae2e7-110">Value</span></span>|<span data-ttu-id="ae2e7-111">説明</span><span class="sxs-lookup"><span data-stu-id="ae2e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae2e7-112">none</span><span class="sxs-lookup"><span data-stu-id="ae2e7-112">none</span></span>|<span data-ttu-id="ae2e7-113">0</span><span class="sxs-lookup"><span data-stu-id="ae2e7-113">0</span></span>|<span data-ttu-id="ae2e7-114">失効していません。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-114">Not revoked.</span></span>|
|<span data-ttu-id="ae2e7-115">保留中</span><span class="sxs-lookup"><span data-stu-id="ae2e7-115">pending</span></span>|<span data-ttu-id="ae2e7-116">1</span><span class="sxs-lookup"><span data-stu-id="ae2e7-116">1</span></span>|<span data-ttu-id="ae2e7-117">保留中の失効します。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-117">Revocation pending.</span></span>|
|<span data-ttu-id="ae2e7-118">発行</span><span class="sxs-lookup"><span data-stu-id="ae2e7-118">issued</span></span>|<span data-ttu-id="ae2e7-119">2</span><span class="sxs-lookup"><span data-stu-id="ae2e7-119">2</span></span>|<span data-ttu-id="ae2e7-120">取り消しコマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-120">Revocation command issued.</span></span>|
|<span data-ttu-id="ae2e7-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-121">failed</span></span>|<span data-ttu-id="ae2e7-122">3</span><span class="sxs-lookup"><span data-stu-id="ae2e7-122">3</span></span>|<span data-ttu-id="ae2e7-123">失効が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-123">Revocation failed.</span></span>|
|<span data-ttu-id="ae2e7-124">失効</span><span class="sxs-lookup"><span data-stu-id="ae2e7-124">revoked</span></span>|<span data-ttu-id="ae2e7-125">4</span><span class="sxs-lookup"><span data-stu-id="ae2e7-125">4</span></span>|<span data-ttu-id="ae2e7-126">無効にします。</span><span class="sxs-lookup"><span data-stu-id="ae2e7-126">Revoked.</span></span>|





