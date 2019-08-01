---
title: defenderCloudBlockLevelType 列挙型
description: クラウドブロックレベルの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 908ebaef963b4c7d8baaf8f1cb0ecfb316d33ad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031879"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="a4464-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a4464-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="a4464-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4464-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4464-105">クラウドブロックレベルの可能な値</span><span class="sxs-lookup"><span data-stu-id="a4464-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="a4464-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a4464-106">Members</span></span>
|<span data-ttu-id="a4464-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a4464-107">Member</span></span>|<span data-ttu-id="a4464-108">値</span><span class="sxs-lookup"><span data-stu-id="a4464-108">Value</span></span>|<span data-ttu-id="a4464-109">説明</span><span class="sxs-lookup"><span data-stu-id="a4464-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4464-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a4464-110">notConfigured</span></span>|<span data-ttu-id="a4464-111">.0</span><span class="sxs-lookup"><span data-stu-id="a4464-111">0</span></span>|<span data-ttu-id="a4464-112">既定値は、Windows Defender ウイルス対策の既定のブロックレベルを使用し、正当なファイルを検出するリスクを増やさずに、強力な検出を提供します。</span><span class="sxs-lookup"><span data-stu-id="a4464-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="a4464-113">高額</span><span class="sxs-lookup"><span data-stu-id="a4464-113">high</span></span>|<span data-ttu-id="a4464-114">1-d</span><span class="sxs-lookup"><span data-stu-id="a4464-114">1</span></span>|<span data-ttu-id="a4464-115">High は、強力なレベルの検出を適用します。</span><span class="sxs-lookup"><span data-stu-id="a4464-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="a4464-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="a4464-116">highPlus</span></span>|<span data-ttu-id="a4464-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a4464-117">2</span></span>|<span data-ttu-id="a4464-118">高 + は高レベルを使用し、追加の保護対策を適用します。</span><span class="sxs-lookup"><span data-stu-id="a4464-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="a4464-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="a4464-119">zeroTolerance</span></span>|<span data-ttu-id="a4464-120">1/3</span><span class="sxs-lookup"><span data-stu-id="a4464-120">3</span></span>|<span data-ttu-id="a4464-121">ゼロトレランスによってすべての不明な実行可能ファイルがブロック</span><span class="sxs-lookup"><span data-stu-id="a4464-121">Zero tolerance blocks all unknown executables</span></span>|



