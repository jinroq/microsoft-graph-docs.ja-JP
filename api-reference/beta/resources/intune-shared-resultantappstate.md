---
title: Resultの重要 Appstate 列挙型
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 712e6039d276d78c187e6e97128a45aa04e62058
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347893"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="cda95-103">Resultの重要 Appstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="cda95-103">resultantAppState enum type</span></span>

> <span data-ttu-id="cda95-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cda95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cda95-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cda95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cda95-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cda95-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="cda95-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="cda95-107">Members</span></span>
|<span data-ttu-id="cda95-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="cda95-108">Member</span></span>|<span data-ttu-id="cda95-109">値</span><span class="sxs-lookup"><span data-stu-id="cda95-109">Value</span></span>|<span data-ttu-id="cda95-110">説明</span><span class="sxs-lookup"><span data-stu-id="cda95-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cda95-111">れる</span><span class="sxs-lookup"><span data-stu-id="cda95-111">installed</span></span>|<span data-ttu-id="cda95-112">1-d</span><span class="sxs-lookup"><span data-stu-id="cda95-112">1</span></span>|<span data-ttu-id="cda95-113">アプリケーションはエラーなしでインストールされます。</span><span class="sxs-lookup"><span data-stu-id="cda95-113">The application is installed with no errors</span></span>|
|<span data-ttu-id="cda95-114">フェール</span><span class="sxs-lookup"><span data-stu-id="cda95-114">failed</span></span>|<span data-ttu-id="cda95-115">pbm-2</span><span class="sxs-lookup"><span data-stu-id="cda95-115">2</span></span>|<span data-ttu-id="cda95-116">アプリケーションをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="cda95-116">The application failed to install.</span></span>|
|<span data-ttu-id="cda95-117">notInstalled</span><span class="sxs-lookup"><span data-stu-id="cda95-117">notInstalled</span></span>|<span data-ttu-id="cda95-118">1/3</span><span class="sxs-lookup"><span data-stu-id="cda95-118">3</span></span>|<span data-ttu-id="cda95-119">アプリケーションがインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="cda95-119">The application is not installed.</span></span>|
|<span data-ttu-id="cda95-120">アンインストールの失敗</span><span class="sxs-lookup"><span data-stu-id="cda95-120">uninstallFailed</span></span>|<span data-ttu-id="cda95-121">2/4</span><span class="sxs-lookup"><span data-stu-id="cda95-121">4</span></span>|<span data-ttu-id="cda95-122">アプリケーションをアンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="cda95-122">The application failed to uninstall.</span></span>|
|<span data-ttu-id="cda95-123">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="cda95-123">pendingInstall</span></span>|<span data-ttu-id="cda95-124">5</span><span class="sxs-lookup"><span data-stu-id="cda95-124">5</span></span>|<span data-ttu-id="cda95-125">アプリケーションのインストールが進行中です。</span><span class="sxs-lookup"><span data-stu-id="cda95-125">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="cda95-126">不明</span><span class="sxs-lookup"><span data-stu-id="cda95-126">unknown</span></span>|<span data-ttu-id="cda95-127">99</span><span class="sxs-lookup"><span data-stu-id="cda95-127">99</span></span>|<span data-ttu-id="cda95-128">アプリケーションの状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="cda95-128">The status of the application is unknown.</span></span>|
|<span data-ttu-id="cda95-129">notApplicable</span><span class="sxs-lookup"><span data-stu-id="cda95-129">notApplicable</span></span>|<span data-ttu-id="cda95-130">-1</span><span class="sxs-lookup"><span data-stu-id="cda95-130">-1</span></span>|<span data-ttu-id="cda95-131">アプリケーションは適用されません。</span><span class="sxs-lookup"><span data-stu-id="cda95-131">The application is not applicable.</span></span>|



