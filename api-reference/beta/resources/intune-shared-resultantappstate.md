---
title: resultantAppState 列挙型
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 7b45353867abe77143fb97755aff457e0c81deb8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319426"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="16063-103">resultantAppState 列挙型</span><span class="sxs-lookup"><span data-stu-id="16063-103">resultantAppState enum type</span></span>

> <span data-ttu-id="16063-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16063-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16063-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16063-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16063-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16063-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16063-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="16063-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="16063-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="16063-108">Members</span></span>
|<span data-ttu-id="16063-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="16063-109">Member</span></span>|<span data-ttu-id="16063-110">値</span><span class="sxs-lookup"><span data-stu-id="16063-110">Value</span></span>|<span data-ttu-id="16063-111">説明</span><span class="sxs-lookup"><span data-stu-id="16063-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16063-112">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="16063-112">installed</span></span>|<span data-ttu-id="16063-113">1</span><span class="sxs-lookup"><span data-stu-id="16063-113">1</span></span>|<span data-ttu-id="16063-114">エラーなしでは、アプリケーションをインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="16063-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="16063-115">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="16063-115">failed</span></span>|<span data-ttu-id="16063-116">2</span><span class="sxs-lookup"><span data-stu-id="16063-116">2</span></span>|<span data-ttu-id="16063-117">アプリケーションをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="16063-117">The application failed to install.</span></span>|
|<span data-ttu-id="16063-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="16063-118">notInstalled</span></span>|<span data-ttu-id="16063-119">3</span><span class="sxs-lookup"><span data-stu-id="16063-119">3</span></span>|<span data-ttu-id="16063-120">アプリケーションがインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="16063-120">The application is not installed.</span></span>|
|<span data-ttu-id="16063-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="16063-121">uninstallFailed</span></span>|<span data-ttu-id="16063-122">4</span><span class="sxs-lookup"><span data-stu-id="16063-122">4</span></span>|<span data-ttu-id="16063-123">アプリケーションをアンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="16063-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="16063-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="16063-124">pendingInstall</span></span>|<span data-ttu-id="16063-125">5</span><span class="sxs-lookup"><span data-stu-id="16063-125">5</span></span>|<span data-ttu-id="16063-126">アプリケーションのインストールは進行中です。</span><span class="sxs-lookup"><span data-stu-id="16063-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="16063-127">不明</span><span class="sxs-lookup"><span data-stu-id="16063-127">unknown</span></span>|<span data-ttu-id="16063-128">99</span><span class="sxs-lookup"><span data-stu-id="16063-128">99</span></span>|<span data-ttu-id="16063-129">アプリケーションのステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="16063-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="16063-130">質問表</span><span class="sxs-lookup"><span data-stu-id="16063-130">notApplicable</span></span>|<span data-ttu-id="16063-131">-1</span><span class="sxs-lookup"><span data-stu-id="16063-131">-1</span></span>|<span data-ttu-id="16063-132">アプリケーションには適用できません。</span><span class="sxs-lookup"><span data-stu-id="16063-132">The application is not applicable.</span></span>|




