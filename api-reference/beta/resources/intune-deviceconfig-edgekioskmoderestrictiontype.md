---
title: edgeKioskModeRestrictionType 列挙型
description: Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ff024dd8cd27872d0895068fba42e0018fdce011
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332513"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="fb405-103">edgeKioskModeRestrictionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="fb405-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="fb405-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fb405-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb405-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fb405-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb405-106">Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb405-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="fb405-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="fb405-107">Members</span></span>
|<span data-ttu-id="fb405-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fb405-108">Member</span></span>|<span data-ttu-id="fb405-109">値</span><span class="sxs-lookup"><span data-stu-id="fb405-109">Value</span></span>|<span data-ttu-id="fb405-110">説明</span><span class="sxs-lookup"><span data-stu-id="fb405-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb405-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fb405-111">notConfigured</span></span>|<span data-ttu-id="fb405-112">.0</span><span class="sxs-lookup"><span data-stu-id="fb405-112">0</span></span>|<span data-ttu-id="fb405-113">未構成 (無制限)。</span><span class="sxs-lookup"><span data-stu-id="fb405-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="fb405-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="fb405-114">digitalSignage</span></span>|<span data-ttu-id="fb405-115">1-d</span><span class="sxs-lookup"><span data-stu-id="fb405-115">1</span></span>|<span data-ttu-id="fb405-116">シングルアプリモードでのインタラクティブ/デジタル信号。</span><span class="sxs-lookup"><span data-stu-id="fb405-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="fb405-117">normalMode</span><span class="sxs-lookup"><span data-stu-id="fb405-117">normalMode</span></span>|<span data-ttu-id="fb405-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="fb405-118">2</span></span>|<span data-ttu-id="fb405-119">標準モード (完全版の Microsoft Edge)。</span><span class="sxs-lookup"><span data-stu-id="fb405-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="fb405-120">Publicた Singsingleapp</span><span class="sxs-lookup"><span data-stu-id="fb405-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="fb405-121">1/3</span><span class="sxs-lookup"><span data-stu-id="fb405-121">3</span></span>|<span data-ttu-id="fb405-122">単一アプリモードでのパブリックブラウズ。</span><span class="sxs-lookup"><span data-stu-id="fb405-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="fb405-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="fb405-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="fb405-124">2/4</span><span class="sxs-lookup"><span data-stu-id="fb405-124">4</span></span>|<span data-ttu-id="fb405-125">マルチアプリモードでのパブリックブラウズ (inPrivate)。</span><span class="sxs-lookup"><span data-stu-id="fb405-125">Public browsing (inPrivate) in multi-app mode.</span></span>|



