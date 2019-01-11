---
title: certificateRevocationStatus 列挙型
description: 証明書失効の状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d24d515f992ed396c3530595240a107852d83e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868307"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="f8821-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="f8821-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="f8821-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f8821-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8821-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8821-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8821-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8821-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8821-107">証明書失効の状態です。</span><span class="sxs-lookup"><span data-stu-id="f8821-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="f8821-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8821-108">Members</span></span>
|<span data-ttu-id="f8821-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8821-109">Member</span></span>|<span data-ttu-id="f8821-110">値</span><span class="sxs-lookup"><span data-stu-id="f8821-110">Value</span></span>|<span data-ttu-id="f8821-111">説明</span><span class="sxs-lookup"><span data-stu-id="f8821-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8821-112">none</span><span class="sxs-lookup"><span data-stu-id="f8821-112">none</span></span>|<span data-ttu-id="f8821-113">0</span><span class="sxs-lookup"><span data-stu-id="f8821-113">0</span></span>|<span data-ttu-id="f8821-114">失効していません。</span><span class="sxs-lookup"><span data-stu-id="f8821-114">Not revoked.</span></span>|
|<span data-ttu-id="f8821-115">保留中</span><span class="sxs-lookup"><span data-stu-id="f8821-115">pending</span></span>|<span data-ttu-id="f8821-116">1</span><span class="sxs-lookup"><span data-stu-id="f8821-116">1</span></span>|<span data-ttu-id="f8821-117">保留中の失効します。</span><span class="sxs-lookup"><span data-stu-id="f8821-117">Revocation pending.</span></span>|
|<span data-ttu-id="f8821-118">発行</span><span class="sxs-lookup"><span data-stu-id="f8821-118">issued</span></span>|<span data-ttu-id="f8821-119">2</span><span class="sxs-lookup"><span data-stu-id="f8821-119">2</span></span>|<span data-ttu-id="f8821-120">取り消しコマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="f8821-120">Revocation command issued.</span></span>|
|<span data-ttu-id="f8821-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="f8821-121">failed</span></span>|<span data-ttu-id="f8821-122">3</span><span class="sxs-lookup"><span data-stu-id="f8821-122">3</span></span>|<span data-ttu-id="f8821-123">失効が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="f8821-123">Revocation failed.</span></span>|
|<span data-ttu-id="f8821-124">失効</span><span class="sxs-lookup"><span data-stu-id="f8821-124">revoked</span></span>|<span data-ttu-id="f8821-125">4</span><span class="sxs-lookup"><span data-stu-id="f8821-125">4</span></span>|<span data-ttu-id="f8821-126">無効にします。</span><span class="sxs-lookup"><span data-stu-id="f8821-126">Revoked.</span></span>|





