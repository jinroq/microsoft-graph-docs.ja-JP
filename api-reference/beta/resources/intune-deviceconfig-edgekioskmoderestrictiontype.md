---
title: edgeKioskModeRestrictionType 列挙型
description: Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dc2aa6dbea5e5fc068691c7de878321047c967d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989827"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a><span data-ttu-id="efc65-103">edgeKioskModeRestrictionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="efc65-103">edgeKioskModeRestrictionType enum type</span></span>

> <span data-ttu-id="efc65-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="efc65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efc65-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="efc65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efc65-106">Microsoft Edge の設定がキオスクモードに基づいて制限される方法を指定します。</span><span class="sxs-lookup"><span data-stu-id="efc65-106">Specify how the Microsoft Edge settings are restricted based on kiosk mode.</span></span>

## <a name="members"></a><span data-ttu-id="efc65-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="efc65-107">Members</span></span>
|<span data-ttu-id="efc65-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="efc65-108">Member</span></span>|<span data-ttu-id="efc65-109">値</span><span class="sxs-lookup"><span data-stu-id="efc65-109">Value</span></span>|<span data-ttu-id="efc65-110">説明</span><span class="sxs-lookup"><span data-stu-id="efc65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efc65-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="efc65-111">notConfigured</span></span>|<span data-ttu-id="efc65-112">.0</span><span class="sxs-lookup"><span data-stu-id="efc65-112">0</span></span>|<span data-ttu-id="efc65-113">未構成 (無制限)。</span><span class="sxs-lookup"><span data-stu-id="efc65-113">Not configured (unrestricted).</span></span>|
|<span data-ttu-id="efc65-114">digitalSignage</span><span class="sxs-lookup"><span data-stu-id="efc65-114">digitalSignage</span></span>|<span data-ttu-id="efc65-115">1-d</span><span class="sxs-lookup"><span data-stu-id="efc65-115">1</span></span>|<span data-ttu-id="efc65-116">シングルアプリモードでのインタラクティブ/デジタル信号。</span><span class="sxs-lookup"><span data-stu-id="efc65-116">Interactive/Digital signage in single-app mode.</span></span>|
|<span data-ttu-id="efc65-117">normalMode</span><span class="sxs-lookup"><span data-stu-id="efc65-117">normalMode</span></span>|<span data-ttu-id="efc65-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="efc65-118">2</span></span>|<span data-ttu-id="efc65-119">標準モード (完全版の Microsoft Edge)。</span><span class="sxs-lookup"><span data-stu-id="efc65-119">Normal mode (full version of Microsoft Edge).</span></span>|
|<span data-ttu-id="efc65-120">Publicた Singsingleapp</span><span class="sxs-lookup"><span data-stu-id="efc65-120">publicBrowsingSingleApp</span></span>|<span data-ttu-id="efc65-121">1/3</span><span class="sxs-lookup"><span data-stu-id="efc65-121">3</span></span>|<span data-ttu-id="efc65-122">単一アプリモードでのパブリックブラウズ。</span><span class="sxs-lookup"><span data-stu-id="efc65-122">Public browsing in single-app mode.</span></span>|
|<span data-ttu-id="efc65-123">publicBrowsingMultiApp</span><span class="sxs-lookup"><span data-stu-id="efc65-123">publicBrowsingMultiApp</span></span>|<span data-ttu-id="efc65-124">2/4</span><span class="sxs-lookup"><span data-stu-id="efc65-124">4</span></span>|<span data-ttu-id="efc65-125">マルチアプリモードでのパブリックブラウズ (inPrivate)。</span><span class="sxs-lookup"><span data-stu-id="efc65-125">Public browsing (inPrivate) in multi-app mode.</span></span>|





