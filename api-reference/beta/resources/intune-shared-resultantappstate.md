---
title: resultantAppState 列挙型
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b97f8f9fc44faf0c27c31f8bab60103547fcf743
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947289"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="4a3ea-103">resultantAppState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4a3ea-103">resultantAppState enum type</span></span>

> <span data-ttu-id="4a3ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a3ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a3ea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a3ea-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4a3ea-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="4a3ea-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a3ea-108">Members</span></span>
|<span data-ttu-id="4a3ea-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4a3ea-109">Member</span></span>|<span data-ttu-id="4a3ea-110">値</span><span class="sxs-lookup"><span data-stu-id="4a3ea-110">Value</span></span>|<span data-ttu-id="4a3ea-111">説明</span><span class="sxs-lookup"><span data-stu-id="4a3ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a3ea-112">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-112">installed</span></span>|<span data-ttu-id="4a3ea-113">1</span><span class="sxs-lookup"><span data-stu-id="4a3ea-113">1</span></span>|<span data-ttu-id="4a3ea-114">エラーなしでは、アプリケーションをインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="4a3ea-115">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-115">failed</span></span>|<span data-ttu-id="4a3ea-116">2</span><span class="sxs-lookup"><span data-stu-id="4a3ea-116">2</span></span>|<span data-ttu-id="4a3ea-117">アプリケーションをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-117">The application failed to install.</span></span>|
|<span data-ttu-id="4a3ea-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="4a3ea-118">notInstalled</span></span>|<span data-ttu-id="4a3ea-119">3</span><span class="sxs-lookup"><span data-stu-id="4a3ea-119">3</span></span>|<span data-ttu-id="4a3ea-120">アプリケーションがインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-120">The application is not installed.</span></span>|
|<span data-ttu-id="4a3ea-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="4a3ea-121">uninstallFailed</span></span>|<span data-ttu-id="4a3ea-122">4</span><span class="sxs-lookup"><span data-stu-id="4a3ea-122">4</span></span>|<span data-ttu-id="4a3ea-123">アプリケーションをアンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="4a3ea-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="4a3ea-124">pendingInstall</span></span>|<span data-ttu-id="4a3ea-125">5</span><span class="sxs-lookup"><span data-stu-id="4a3ea-125">5</span></span>|<span data-ttu-id="4a3ea-126">アプリケーションのインストールは進行中です。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="4a3ea-127">不明</span><span class="sxs-lookup"><span data-stu-id="4a3ea-127">unknown</span></span>|<span data-ttu-id="4a3ea-128">99</span><span class="sxs-lookup"><span data-stu-id="4a3ea-128">99</span></span>|<span data-ttu-id="4a3ea-129">アプリケーションのステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="4a3ea-130">質問表</span><span class="sxs-lookup"><span data-stu-id="4a3ea-130">notApplicable</span></span>|<span data-ttu-id="4a3ea-131">-1</span><span class="sxs-lookup"><span data-stu-id="4a3ea-131">-1</span></span>|<span data-ttu-id="4a3ea-132">アプリケーションには適用できません。</span><span class="sxs-lookup"><span data-stu-id="4a3ea-132">The application is not applicable.</span></span>|





