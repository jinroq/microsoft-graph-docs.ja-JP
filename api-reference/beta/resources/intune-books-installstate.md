---
title: installState 列挙型
description: インストール状態の値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1c3a1d86257611cb00d8ee2c4ee0b8173b03f197
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425877"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="6f5c1-103">installState 列挙型</span><span class="sxs-lookup"><span data-stu-id="6f5c1-103">installState enum type</span></span>

> <span data-ttu-id="6f5c1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f5c1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f5c1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f5c1-107">インストール状態の値です。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-107">Possible values for install state.</span></span>

## <a name="members"></a><span data-ttu-id="6f5c1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6f5c1-108">Members</span></span>
|<span data-ttu-id="6f5c1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6f5c1-109">Member</span></span>|<span data-ttu-id="6f5c1-110">値</span><span class="sxs-lookup"><span data-stu-id="6f5c1-110">Value</span></span>|<span data-ttu-id="6f5c1-111">説明</span><span class="sxs-lookup"><span data-stu-id="6f5c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f5c1-112">質問表</span><span class="sxs-lookup"><span data-stu-id="6f5c1-112">notApplicable</span></span>|<span data-ttu-id="6f5c1-113">0</span><span class="sxs-lookup"><span data-stu-id="6f5c1-113">0</span></span>|<span data-ttu-id="6f5c1-114">適用されません。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-114">Not Applicable.</span></span>|
|<span data-ttu-id="6f5c1-115">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-115">installed</span></span>|<span data-ttu-id="6f5c1-116">1</span><span class="sxs-lookup"><span data-stu-id="6f5c1-116">1</span></span>|<span data-ttu-id="6f5c1-117">インストールされています。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-117">Installed.</span></span>|
|<span data-ttu-id="6f5c1-118">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-118">failed</span></span>|<span data-ttu-id="6f5c1-119">2</span><span class="sxs-lookup"><span data-stu-id="6f5c1-119">2</span></span>|<span data-ttu-id="6f5c1-120">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-120">Failed.</span></span>|
|<span data-ttu-id="6f5c1-121">notInstalled</span><span class="sxs-lookup"><span data-stu-id="6f5c1-121">notInstalled</span></span>|<span data-ttu-id="6f5c1-122">3</span><span class="sxs-lookup"><span data-stu-id="6f5c1-122">3</span></span>|<span data-ttu-id="6f5c1-123">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-123">Not Installed.</span></span>|
|<span data-ttu-id="6f5c1-124">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="6f5c1-124">uninstallFailed</span></span>|<span data-ttu-id="6f5c1-125">4</span><span class="sxs-lookup"><span data-stu-id="6f5c1-125">4</span></span>|<span data-ttu-id="6f5c1-126">アンインストールできませんでした。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-126">Uninstall Failed.</span></span>|
|<span data-ttu-id="6f5c1-127">不明</span><span class="sxs-lookup"><span data-stu-id="6f5c1-127">unknown</span></span>|<span data-ttu-id="6f5c1-128">5</span><span class="sxs-lookup"><span data-stu-id="6f5c1-128">5</span></span>|<span data-ttu-id="6f5c1-129">不明。</span><span class="sxs-lookup"><span data-stu-id="6f5c1-129">Unknown.</span></span>|




