---
title: resultantAppState 列挙型
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf3d7e8ef20b1458811ae1a49b23120f7cd153d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422685"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="72d87-103">resultantAppState 列挙型</span><span class="sxs-lookup"><span data-stu-id="72d87-103">resultantAppState enum type</span></span>

> <span data-ttu-id="72d87-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="72d87-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72d87-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72d87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72d87-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="72d87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72d87-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="72d87-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="72d87-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="72d87-108">Members</span></span>
|<span data-ttu-id="72d87-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="72d87-109">Member</span></span>|<span data-ttu-id="72d87-110">値</span><span class="sxs-lookup"><span data-stu-id="72d87-110">Value</span></span>|<span data-ttu-id="72d87-111">説明</span><span class="sxs-lookup"><span data-stu-id="72d87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72d87-112">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="72d87-112">installed</span></span>|<span data-ttu-id="72d87-113">1</span><span class="sxs-lookup"><span data-stu-id="72d87-113">1</span></span>|<span data-ttu-id="72d87-114">エラーなしでは、アプリケーションをインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="72d87-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="72d87-115">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="72d87-115">failed</span></span>|<span data-ttu-id="72d87-116">2</span><span class="sxs-lookup"><span data-stu-id="72d87-116">2</span></span>|<span data-ttu-id="72d87-117">アプリケーションをインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="72d87-117">The application failed to install.</span></span>|
|<span data-ttu-id="72d87-118">notInstalled</span><span class="sxs-lookup"><span data-stu-id="72d87-118">notInstalled</span></span>|<span data-ttu-id="72d87-119">3</span><span class="sxs-lookup"><span data-stu-id="72d87-119">3</span></span>|<span data-ttu-id="72d87-120">アプリケーションがインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="72d87-120">The application is not installed.</span></span>|
|<span data-ttu-id="72d87-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="72d87-121">uninstallFailed</span></span>|<span data-ttu-id="72d87-122">4</span><span class="sxs-lookup"><span data-stu-id="72d87-122">4</span></span>|<span data-ttu-id="72d87-123">アプリケーションをアンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="72d87-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="72d87-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="72d87-124">pendingInstall</span></span>|<span data-ttu-id="72d87-125">5</span><span class="sxs-lookup"><span data-stu-id="72d87-125">5</span></span>|<span data-ttu-id="72d87-126">アプリケーションのインストールは進行中です。</span><span class="sxs-lookup"><span data-stu-id="72d87-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="72d87-127">不明</span><span class="sxs-lookup"><span data-stu-id="72d87-127">unknown</span></span>|<span data-ttu-id="72d87-128">99</span><span class="sxs-lookup"><span data-stu-id="72d87-128">99</span></span>|<span data-ttu-id="72d87-129">アプリケーションのステータスは不明です。</span><span class="sxs-lookup"><span data-stu-id="72d87-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="72d87-130">質問表</span><span class="sxs-lookup"><span data-stu-id="72d87-130">notApplicable</span></span>|<span data-ttu-id="72d87-131">-1</span><span class="sxs-lookup"><span data-stu-id="72d87-131">-1</span></span>|<span data-ttu-id="72d87-132">アプリケーションには適用できません。</span><span class="sxs-lookup"><span data-stu-id="72d87-132">The application is not applicable.</span></span>|




