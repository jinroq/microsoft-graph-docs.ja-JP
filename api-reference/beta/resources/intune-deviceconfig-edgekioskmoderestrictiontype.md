---
title: edgeKioskModeRestrictionType 列挙型
description: Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74b03555456c058411c9a50c7392f29fe60d3aed
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799546"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="a9ab4-103">edgeKioskModeRestrictionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a9ab4-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="a9ab4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9ab4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9ab4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9ab4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9ab4-106">Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9ab4-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="a9ab4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a9ab4-107">Members</span></span>
|<span data-ttu-id="a9ab4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a9ab4-108">Member</span></span>|<span data-ttu-id="a9ab4-109">値</span><span class="sxs-lookup"><span data-stu-id="a9ab4-109">Value</span></span>|<span data-ttu-id="a9ab4-110">説明</span><span class="sxs-lookup"><span data-stu-id="a9ab4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9ab4-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a9ab4-111">notConfigured</span></span>|<span data-ttu-id="a9ab4-112">.0</span><span class="sxs-lookup"><span data-stu-id="a9ab4-112">0</span></span>|<span data-ttu-id="a9ab4-113">未構成 (無制限)。</span><span class="sxs-lookup"><span data-stu-id="a9ab4-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="a9ab4-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="a9ab4-114">digitalSignage</span></span>|<span data-ttu-id="a9ab4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a9ab4-115">1</span></span>|<span data-ttu-id="a9ab4-116">シングルアプリモードでのインタラクティブ/デジタル信号。</span><span class="sxs-lookup"><span data-stu-id="a9ab4-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="a9ab4-117">normalmode</span><span class="sxs-lookup"><span data-stu-id="a9ab4-117">normalMode</span></span>|<span data-ttu-id="a9ab4-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a9ab4-118">2</span></span>|<span data-ttu-id="a9ab4-119">標準モード (完全版の Microsoft Edge)。</span><span class="sxs-lookup"><span data-stu-id="a9ab4-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="a9ab4-120">publicた singsingleapp</span><span class="sxs-lookup"><span data-stu-id="a9ab4-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="a9ab4-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a9ab4-121">3</span></span>|<span data-ttu-id="a9ab4-122">単一アプリモードでのパブリックブラウズ。</span><span class="sxs-lookup"><span data-stu-id="a9ab4-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="a9ab4-123">publicbrowsingmultiapp</span><span class="sxs-lookup"><span data-stu-id="a9ab4-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="a9ab4-124">2/4</span><span class="sxs-lookup"><span data-stu-id="a9ab4-124">4</span></span>|<span data-ttu-id="a9ab4-125">マルチアプリモードでのパブリックブラウズ (inPrivate)。</span><span class="sxs-lookup"><span data-stu-id="a9ab4-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





