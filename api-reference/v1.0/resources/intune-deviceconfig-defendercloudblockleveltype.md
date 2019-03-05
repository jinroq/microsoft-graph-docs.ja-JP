---
title: defendercloudblockleveltype 列挙型
description: クラウドブロックレベルの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258836"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="32fb5-103">defendercloudblockleveltype 列挙型</span><span class="sxs-lookup"><span data-stu-id="32fb5-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="32fb5-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="32fb5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32fb5-105">クラウドブロックレベルの可能な値</span><span class="sxs-lookup"><span data-stu-id="32fb5-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="32fb5-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="32fb5-106">Members</span></span>
|<span data-ttu-id="32fb5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="32fb5-107">Member</span></span>|<span data-ttu-id="32fb5-108">値</span><span class="sxs-lookup"><span data-stu-id="32fb5-108">Value</span></span>|<span data-ttu-id="32fb5-109">説明</span><span class="sxs-lookup"><span data-stu-id="32fb5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32fb5-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="32fb5-110">notConfigured</span></span>|<span data-ttu-id="32fb5-111">.0</span><span class="sxs-lookup"><span data-stu-id="32fb5-111">0</span></span>|<span data-ttu-id="32fb5-112">既定値は、Windows Defender ウイルス対策の既定のブロックレベルを使用し、正当なファイルを検出するリスクを増やさずに、強力な検出を提供します。</span><span class="sxs-lookup"><span data-stu-id="32fb5-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="32fb5-113">高額</span><span class="sxs-lookup"><span data-stu-id="32fb5-113">high</span></span>|<span data-ttu-id="32fb5-114">1-d</span><span class="sxs-lookup"><span data-stu-id="32fb5-114">1</span></span>|<span data-ttu-id="32fb5-115">High は、強力なレベルの検出を適用します。</span><span class="sxs-lookup"><span data-stu-id="32fb5-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="32fb5-116">highplus</span><span class="sxs-lookup"><span data-stu-id="32fb5-116">highPlus</span></span>|<span data-ttu-id="32fb5-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="32fb5-117">2</span></span>|<span data-ttu-id="32fb5-118">高 + は高レベルを使用し、追加の保護対策を適用します。</span><span class="sxs-lookup"><span data-stu-id="32fb5-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="32fb5-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="32fb5-119">zeroTolerance</span></span>|<span data-ttu-id="32fb5-120">1/3</span><span class="sxs-lookup"><span data-stu-id="32fb5-120">3</span></span>|<span data-ttu-id="32fb5-121">ゼロトレランスによってすべての不明な実行可能ファイルがブロック</span><span class="sxs-lookup"><span data-stu-id="32fb5-121">Zero tolerance blocks all unknown executables</span></span>|



