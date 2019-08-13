---
title: defenderCloudBlockLevelType 列挙型
description: クラウドブロックレベルの可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc0e99f9d964e80410b10bc48e20ea0a5fd1d608
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333591"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="e9830-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e9830-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="e9830-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9830-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9830-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9830-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9830-106">クラウドブロックレベルの可能な値</span><span class="sxs-lookup"><span data-stu-id="e9830-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="e9830-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e9830-107">Members</span></span>
|<span data-ttu-id="e9830-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e9830-108">Member</span></span>|<span data-ttu-id="e9830-109">値</span><span class="sxs-lookup"><span data-stu-id="e9830-109">Value</span></span>|<span data-ttu-id="e9830-110">説明</span><span class="sxs-lookup"><span data-stu-id="e9830-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9830-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e9830-111">notConfigured</span></span>|<span data-ttu-id="e9830-112">.0</span><span class="sxs-lookup"><span data-stu-id="e9830-112">0</span></span>|<span data-ttu-id="e9830-113">既定値は、Windows Defender ウイルス対策の既定のブロックレベルを使用し、正当なファイルを検出するリスクを増やさずに、強力な検出を提供します。</span><span class="sxs-lookup"><span data-stu-id="e9830-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="e9830-114">高額</span><span class="sxs-lookup"><span data-stu-id="e9830-114">high</span></span>|<span data-ttu-id="e9830-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e9830-115">1</span></span>|<span data-ttu-id="e9830-116">High は、強力なレベルの検出を適用します。</span><span class="sxs-lookup"><span data-stu-id="e9830-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="e9830-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="e9830-117">highPlus</span></span>|<span data-ttu-id="e9830-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e9830-118">2</span></span>|<span data-ttu-id="e9830-119">高 + は高レベルを使用し、追加の保護対策を適用します。</span><span class="sxs-lookup"><span data-stu-id="e9830-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="e9830-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="e9830-120">zeroTolerance</span></span>|<span data-ttu-id="e9830-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e9830-121">3</span></span>|<span data-ttu-id="e9830-122">ゼロトレランスによってすべての不明な実行可能ファイルがブロック</span><span class="sxs-lookup"><span data-stu-id="e9830-122">Zero tolerance blocks all unknown executables</span></span>|



