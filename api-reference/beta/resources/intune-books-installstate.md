---
title: installState 列挙型
description: インストール状態の値です。
ms.openlocfilehash: c452deb5bc04e944139870d0ccceebc65a91ac1e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067529"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="9977f-103">installState 列挙型</span><span class="sxs-lookup"><span data-stu-id="9977f-103">installState enum type</span></span>

> <span data-ttu-id="9977f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9977f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9977f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9977f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9977f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9977f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9977f-107">インストール状態の値です。</span><span class="sxs-lookup"><span data-stu-id="9977f-107">Possible values for install state.</span></span>
## <a name="members"></a><span data-ttu-id="9977f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9977f-108">Members</span></span>
|<span data-ttu-id="9977f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9977f-109">Member</span></span>|<span data-ttu-id="9977f-110">値</span><span class="sxs-lookup"><span data-stu-id="9977f-110">Value</span></span>|<span data-ttu-id="9977f-111">説明</span><span class="sxs-lookup"><span data-stu-id="9977f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9977f-112">質問表</span><span class="sxs-lookup"><span data-stu-id="9977f-112">notApplicable</span></span>|<span data-ttu-id="9977f-113">0</span><span class="sxs-lookup"><span data-stu-id="9977f-113">0</span></span>|<span data-ttu-id="9977f-114">適用されません。</span><span class="sxs-lookup"><span data-stu-id="9977f-114">Not Applicable.</span></span>|
|<span data-ttu-id="9977f-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="9977f-115">installed</span></span>|<span data-ttu-id="9977f-116">1</span><span class="sxs-lookup"><span data-stu-id="9977f-116">1</span></span>|<span data-ttu-id="9977f-117">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="9977f-117">Installed.</span></span>|
|<span data-ttu-id="9977f-118">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9977f-118">failed</span></span>|<span data-ttu-id="9977f-119">2</span><span class="sxs-lookup"><span data-stu-id="9977f-119">2</span></span>|<span data-ttu-id="9977f-120">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9977f-120">Failed.</span></span>|
|<span data-ttu-id="9977f-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="9977f-121">notInstalled</span></span>|<span data-ttu-id="9977f-122">3</span><span class="sxs-lookup"><span data-stu-id="9977f-122">3</span></span>|<span data-ttu-id="9977f-123">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="9977f-123">Not Installed.</span></span>|
|<span data-ttu-id="9977f-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="9977f-124">uninstallFailed</span></span>|<span data-ttu-id="9977f-125">4</span><span class="sxs-lookup"><span data-stu-id="9977f-125">4</span></span>|<span data-ttu-id="9977f-126">アンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="9977f-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="9977f-127">不明</span><span class="sxs-lookup"><span data-stu-id="9977f-127">unknown</span></span>|<span data-ttu-id="9977f-128">5</span><span class="sxs-lookup"><span data-stu-id="9977f-128">5</span></span>|<span data-ttu-id="9977f-129">不明。</span><span class="sxs-lookup"><span data-stu-id="9977f-129">Unknown.</span></span>|





