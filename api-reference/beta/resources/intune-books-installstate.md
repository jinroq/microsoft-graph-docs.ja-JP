---
title: installState 列挙型
description: インストール状態の値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa281cc5f218469980a235db842e00fd8fa46647
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868622"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="cbd2e-103">installState 列挙型</span><span class="sxs-lookup"><span data-stu-id="cbd2e-103">installState enum type</span></span>

> <span data-ttu-id="cbd2e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbd2e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbd2e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbd2e-107">インストール状態の値です。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="cbd2e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="cbd2e-108">Members</span></span>
|<span data-ttu-id="cbd2e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="cbd2e-109">Member</span></span>|<span data-ttu-id="cbd2e-110">値</span><span class="sxs-lookup"><span data-stu-id="cbd2e-110">Value</span></span>|<span data-ttu-id="cbd2e-111">説明</span><span class="sxs-lookup"><span data-stu-id="cbd2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbd2e-112">質問表</span><span class="sxs-lookup"><span data-stu-id="cbd2e-112">notApplicable</span></span>|<span data-ttu-id="cbd2e-113">0</span><span class="sxs-lookup"><span data-stu-id="cbd2e-113">0</span></span>|<span data-ttu-id="cbd2e-114">適用されません。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-114">Not Applicable.</span></span>|
|<span data-ttu-id="cbd2e-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-115">installed</span></span>|<span data-ttu-id="cbd2e-116">1</span><span class="sxs-lookup"><span data-stu-id="cbd2e-116">1</span></span>|<span data-ttu-id="cbd2e-117">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-117">Installed.</span></span>|
|<span data-ttu-id="cbd2e-118">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-118">failed</span></span>|<span data-ttu-id="cbd2e-119">2</span><span class="sxs-lookup"><span data-stu-id="cbd2e-119">2</span></span>|<span data-ttu-id="cbd2e-120">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-120">Failed.</span></span>|
|<span data-ttu-id="cbd2e-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="cbd2e-121">notInstalled</span></span>|<span data-ttu-id="cbd2e-122">3</span><span class="sxs-lookup"><span data-stu-id="cbd2e-122">3</span></span>|<span data-ttu-id="cbd2e-123">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-123">Not Installed.</span></span>|
|<span data-ttu-id="cbd2e-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="cbd2e-124">uninstallFailed</span></span>|<span data-ttu-id="cbd2e-125">4</span><span class="sxs-lookup"><span data-stu-id="cbd2e-125">4</span></span>|<span data-ttu-id="cbd2e-126">アンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="cbd2e-127">不明</span><span class="sxs-lookup"><span data-stu-id="cbd2e-127">unknown</span></span>|<span data-ttu-id="cbd2e-128">5</span><span class="sxs-lookup"><span data-stu-id="cbd2e-128">5</span></span>|<span data-ttu-id="cbd2e-129">不明。</span><span class="sxs-lookup"><span data-stu-id="cbd2e-129">Unknown.</span></span>|





