---
title: edgeKioskModeRestrictionType 列挙型
description: Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 014025b04974df90dc6e22e55f3597fc265b207d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946743"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="7faa3-103">edgeKioskModeRestrictionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7faa3-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="7faa3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7faa3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7faa3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7faa3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7faa3-106">Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="7faa3-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="7faa3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7faa3-107">Members</span></span>
|<span data-ttu-id="7faa3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7faa3-108">Member</span></span>|<span data-ttu-id="7faa3-109">値</span><span class="sxs-lookup"><span data-stu-id="7faa3-109">Value</span></span>|<span data-ttu-id="7faa3-110">説明</span><span class="sxs-lookup"><span data-stu-id="7faa3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7faa3-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="7faa3-111">notConfigured</span></span>|<span data-ttu-id="7faa3-112">.0</span><span class="sxs-lookup"><span data-stu-id="7faa3-112">0</span></span>|<span data-ttu-id="7faa3-113">未構成 (無制限)。</span><span class="sxs-lookup"><span data-stu-id="7faa3-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="7faa3-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="7faa3-114">digitalSignage</span></span>|<span data-ttu-id="7faa3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7faa3-115">1</span></span>|<span data-ttu-id="7faa3-116">シングルアプリモードでのインタラクティブ/デジタル信号。</span><span class="sxs-lookup"><span data-stu-id="7faa3-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="7faa3-117">normalMode</span><span class="sxs-lookup"><span data-stu-id="7faa3-117">normalMode</span></span>|<span data-ttu-id="7faa3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7faa3-118">2</span></span>|<span data-ttu-id="7faa3-119">標準モード (完全版の Microsoft Edge)。</span><span class="sxs-lookup"><span data-stu-id="7faa3-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="7faa3-120">Publicた Singsingleapp</span><span class="sxs-lookup"><span data-stu-id="7faa3-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="7faa3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="7faa3-121">3</span></span>|<span data-ttu-id="7faa3-122">単一アプリモードでのパブリックブラウズ。</span><span class="sxs-lookup"><span data-stu-id="7faa3-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="7faa3-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="7faa3-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="7faa3-124">2/4</span><span class="sxs-lookup"><span data-stu-id="7faa3-124">4</span></span>|<span data-ttu-id="7faa3-125">マルチアプリモードでのパブリックブラウズ (inPrivate)。</span><span class="sxs-lookup"><span data-stu-id="7faa3-125">Public browsing (inPrivate) in multi-app mode.</span></span>|




