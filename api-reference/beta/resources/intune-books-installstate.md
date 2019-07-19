---
title: installState 列挙型
description: インストール状態の値を指定できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 26665b5aee40f14ffa6a4d194e706061a35a6bdb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964347"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="21bad-103">installState 列挙型</span><span class="sxs-lookup"><span data-stu-id="21bad-103">installState enum type</span></span>

> <span data-ttu-id="21bad-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21bad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bad-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="21bad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bad-106">インストール状態の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="21bad-106">Possible values for install state.</span></span>

## <a name="members"></a><span data-ttu-id="21bad-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="21bad-107">Members</span></span>
|<span data-ttu-id="21bad-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="21bad-108">Member</span></span>|<span data-ttu-id="21bad-109">値</span><span class="sxs-lookup"><span data-stu-id="21bad-109">Value</span></span>|<span data-ttu-id="21bad-110">説明</span><span class="sxs-lookup"><span data-stu-id="21bad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bad-111">notApplicable</span><span class="sxs-lookup"><span data-stu-id="21bad-111">notApplicable</span></span>|<span data-ttu-id="21bad-112">.0</span><span class="sxs-lookup"><span data-stu-id="21bad-112">0</span></span>|<span data-ttu-id="21bad-113">該当なし。</span><span class="sxs-lookup"><span data-stu-id="21bad-113">Not Applicable.</span></span>|
|<span data-ttu-id="21bad-114">れる</span><span class="sxs-lookup"><span data-stu-id="21bad-114">installed</span></span>|<span data-ttu-id="21bad-115">1-d</span><span class="sxs-lookup"><span data-stu-id="21bad-115">1</span></span>|<span data-ttu-id="21bad-116">れる.</span><span class="sxs-lookup"><span data-stu-id="21bad-116">Installed.</span></span>|
|<span data-ttu-id="21bad-117">フェール</span><span class="sxs-lookup"><span data-stu-id="21bad-117">failed</span></span>|<span data-ttu-id="21bad-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="21bad-118">2</span></span>|<span data-ttu-id="21bad-119">フェール.</span><span class="sxs-lookup"><span data-stu-id="21bad-119">Failed.</span></span>|
|<span data-ttu-id="21bad-120">notInstalled</span><span class="sxs-lookup"><span data-stu-id="21bad-120">notInstalled</span></span>|<span data-ttu-id="21bad-121">1/3</span><span class="sxs-lookup"><span data-stu-id="21bad-121">3</span></span>|<span data-ttu-id="21bad-122">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="21bad-122">Not Installed.</span></span>|
|<span data-ttu-id="21bad-123">アンインストールの失敗</span><span class="sxs-lookup"><span data-stu-id="21bad-123">uninstallFailed</span></span>|<span data-ttu-id="21bad-124">2/4</span><span class="sxs-lookup"><span data-stu-id="21bad-124">4</span></span>|<span data-ttu-id="21bad-125">アンインストールに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="21bad-125">Uninstall Failed.</span></span>|
|<span data-ttu-id="21bad-126">不明</span><span class="sxs-lookup"><span data-stu-id="21bad-126">unknown</span></span>|<span data-ttu-id="21bad-127">5</span><span class="sxs-lookup"><span data-stu-id="21bad-127">5</span></span>|<span data-ttu-id="21bad-128">わかり.</span><span class="sxs-lookup"><span data-stu-id="21bad-128">Unknown.</span></span>|





