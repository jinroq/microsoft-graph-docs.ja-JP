---
title: installstate 列挙型
description: インストール状態の値を指定できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0554df30b4d7165c0164749730e2584af6cc35fd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158213"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="19a16-103">installstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="19a16-103">installState enum type</span></span>

> <span data-ttu-id="19a16-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19a16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19a16-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="19a16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19a16-106">インストール状態の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="19a16-106">Possible values for install state.</span></span>

## <a name="members"></a><span data-ttu-id="19a16-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="19a16-107">Members</span></span>
|<span data-ttu-id="19a16-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="19a16-108">Member</span></span>|<span data-ttu-id="19a16-109">値</span><span class="sxs-lookup"><span data-stu-id="19a16-109">Value</span></span>|<span data-ttu-id="19a16-110">説明</span><span class="sxs-lookup"><span data-stu-id="19a16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19a16-111">notapplicable</span><span class="sxs-lookup"><span data-stu-id="19a16-111">notApplicable</span></span>|<span data-ttu-id="19a16-112">.0</span><span class="sxs-lookup"><span data-stu-id="19a16-112">0</span></span>|<span data-ttu-id="19a16-113">該当なし。</span><span class="sxs-lookup"><span data-stu-id="19a16-113">Not Applicable.</span></span>|
|<span data-ttu-id="19a16-114">れる</span><span class="sxs-lookup"><span data-stu-id="19a16-114">installed</span></span>|<span data-ttu-id="19a16-115">1-d</span><span class="sxs-lookup"><span data-stu-id="19a16-115">1</span></span>|<span data-ttu-id="19a16-116">れる.</span><span class="sxs-lookup"><span data-stu-id="19a16-116">Installed.</span></span>|
|<span data-ttu-id="19a16-117">フェール</span><span class="sxs-lookup"><span data-stu-id="19a16-117">failed</span></span>|<span data-ttu-id="19a16-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="19a16-118">2</span></span>|<span data-ttu-id="19a16-119">フェール.</span><span class="sxs-lookup"><span data-stu-id="19a16-119">Failed.</span></span>|
|<span data-ttu-id="19a16-120">notinstalled</span><span class="sxs-lookup"><span data-stu-id="19a16-120">notInstalled</span></span>|<span data-ttu-id="19a16-121">1/3</span><span class="sxs-lookup"><span data-stu-id="19a16-121">3</span></span>|<span data-ttu-id="19a16-122">インストールされていません。</span><span class="sxs-lookup"><span data-stu-id="19a16-122">Not Installed.</span></span>|
|<span data-ttu-id="19a16-123">アンインストールの失敗</span><span class="sxs-lookup"><span data-stu-id="19a16-123">uninstallFailed</span></span>|<span data-ttu-id="19a16-124">2/4</span><span class="sxs-lookup"><span data-stu-id="19a16-124">4</span></span>|<span data-ttu-id="19a16-125">アンインストールに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="19a16-125">Uninstall Failed.</span></span>|
|<span data-ttu-id="19a16-126">不明</span><span class="sxs-lookup"><span data-stu-id="19a16-126">unknown</span></span>|<span data-ttu-id="19a16-127">5</span><span class="sxs-lookup"><span data-stu-id="19a16-127">5</span></span>|<span data-ttu-id="19a16-128">わかり.</span><span class="sxs-lookup"><span data-stu-id="19a16-128">Unknown.</span></span>|




