---
title: defenderCloudBlockLevelType 列挙型
description: クラウドブロックレベルの可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f798e4b7572cc2593d0d742ecbdebf81d65507d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979866"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="c6134-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c6134-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="c6134-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6134-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6134-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c6134-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6134-106">クラウドブロックレベルの可能な値</span><span class="sxs-lookup"><span data-stu-id="c6134-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="c6134-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c6134-107">Members</span></span>
|<span data-ttu-id="c6134-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c6134-108">Member</span></span>|<span data-ttu-id="c6134-109">値</span><span class="sxs-lookup"><span data-stu-id="c6134-109">Value</span></span>|<span data-ttu-id="c6134-110">説明</span><span class="sxs-lookup"><span data-stu-id="c6134-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6134-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c6134-111">notConfigured</span></span>|<span data-ttu-id="c6134-112">.0</span><span class="sxs-lookup"><span data-stu-id="c6134-112">0</span></span>|<span data-ttu-id="c6134-113">既定値は、Windows Defender ウイルス対策の既定のブロックレベルを使用し、正当なファイルを検出するリスクを増やさずに、強力な検出を提供します。</span><span class="sxs-lookup"><span data-stu-id="c6134-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="c6134-114">高額</span><span class="sxs-lookup"><span data-stu-id="c6134-114">high</span></span>|<span data-ttu-id="c6134-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c6134-115">1</span></span>|<span data-ttu-id="c6134-116">High は、強力なレベルの検出を適用します。</span><span class="sxs-lookup"><span data-stu-id="c6134-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="c6134-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="c6134-117">highPlus</span></span>|<span data-ttu-id="c6134-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c6134-118">2</span></span>|<span data-ttu-id="c6134-119">高 + は高レベルを使用し、追加の保護対策を適用します。</span><span class="sxs-lookup"><span data-stu-id="c6134-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="c6134-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="c6134-120">zeroTolerance</span></span>|<span data-ttu-id="c6134-121">1/3</span><span class="sxs-lookup"><span data-stu-id="c6134-121">3</span></span>|<span data-ttu-id="c6134-122">ゼロトレランスによってすべての不明な実行可能ファイルがブロック</span><span class="sxs-lookup"><span data-stu-id="c6134-122">Zero tolerance blocks all unknown executables</span></span>|





