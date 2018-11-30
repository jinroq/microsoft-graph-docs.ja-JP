---
title: resultantAppState 列挙型
description: まだ文書化されていません
ms.openlocfilehash: 7c3dd96aca4ed94a45a36b9a48a2908f805bb1f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073239"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="43e99-103">resultantAppState 列挙型</span><span class="sxs-lookup"><span data-stu-id="43e99-103">resultantAppState enum type</span></span>

> <span data-ttu-id="43e99-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="43e99-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43e99-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43e99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43e99-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="43e99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43e99-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="43e99-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="43e99-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="43e99-108">Members</span></span>
|<span data-ttu-id="43e99-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="43e99-109">Member</span></span>|<span data-ttu-id="43e99-110">値</span><span class="sxs-lookup"><span data-stu-id="43e99-110">Value</span></span>|<span data-ttu-id="43e99-111">説明</span><span class="sxs-lookup"><span data-stu-id="43e99-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43e99-112">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="43e99-112">installed</span></span>|<span data-ttu-id="43e99-113">1</span><span class="sxs-lookup"><span data-stu-id="43e99-113">1</span></span>|<span data-ttu-id="43e99-114">エラーなしでは、アプリケーションをインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="43e99-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="43e99-115">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="43e99-115">failed</span></span>|<span data-ttu-id="43e99-116">2</span><span class="sxs-lookup"><span data-stu-id="43e99-116">2</span></span>|<span data-ttu-id="43e99-117">アプリケーションをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="43e99-117">The application failed to install.</span></span>|
|<span data-ttu-id="43e99-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="43e99-118">notInstalled</span></span>|<span data-ttu-id="43e99-119">3</span><span class="sxs-lookup"><span data-stu-id="43e99-119">3</span></span>|<span data-ttu-id="43e99-120">アプリケーションがインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="43e99-120">The application is not installed.</span></span>|
|<span data-ttu-id="43e99-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="43e99-121">uninstallFailed</span></span>|<span data-ttu-id="43e99-122">4</span><span class="sxs-lookup"><span data-stu-id="43e99-122">4</span></span>|<span data-ttu-id="43e99-123">アプリケーションをアンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="43e99-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="43e99-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="43e99-124">pendingInstall</span></span>|<span data-ttu-id="43e99-125">5</span><span class="sxs-lookup"><span data-stu-id="43e99-125">5</span></span>|<span data-ttu-id="43e99-126">アプリケーションのインストールは進行中です。</span><span class="sxs-lookup"><span data-stu-id="43e99-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="43e99-127">不明</span><span class="sxs-lookup"><span data-stu-id="43e99-127">unknown</span></span>|<span data-ttu-id="43e99-128">99</span><span class="sxs-lookup"><span data-stu-id="43e99-128">99</span></span>|<span data-ttu-id="43e99-129">アプリケーションのステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="43e99-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="43e99-130">質問表</span><span class="sxs-lookup"><span data-stu-id="43e99-130">notApplicable</span></span>|<span data-ttu-id="43e99-131">-1</span><span class="sxs-lookup"><span data-stu-id="43e99-131">-1</span></span>|<span data-ttu-id="43e99-132">アプリケーションには適用できません。</span><span class="sxs-lookup"><span data-stu-id="43e99-132">The application is not applicable.</span></span>|





