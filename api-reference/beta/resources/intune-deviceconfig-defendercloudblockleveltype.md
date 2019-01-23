---
title: defenderCloudBlockLevelType 列挙型
description: クラウド ・ ブロック ・ レベルで使用できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b309184623cff19e44ee5afea311d46fa89210fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425912"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="104f0-103">defenderCloudBlockLevelType 列挙型</span><span class="sxs-lookup"><span data-stu-id="104f0-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="104f0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="104f0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="104f0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="104f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="104f0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="104f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="104f0-107">クラウド ・ ブロック ・ レベルで使用できる値</span><span class="sxs-lookup"><span data-stu-id="104f0-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="104f0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="104f0-108">Members</span></span>
|<span data-ttu-id="104f0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="104f0-109">Member</span></span>|<span data-ttu-id="104f0-110">値</span><span class="sxs-lookup"><span data-stu-id="104f0-110">Value</span></span>|<span data-ttu-id="104f0-111">説明</span><span class="sxs-lookup"><span data-stu-id="104f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="104f0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="104f0-112">notConfigured</span></span>|<span data-ttu-id="104f0-113">0</span><span class="sxs-lookup"><span data-stu-id="104f0-113">0</span></span>|<span data-ttu-id="104f0-114">既定値、レベルおよび検出のリスクを増大させることがなく強固な検出は、既定の Windows Defender のウイルス対策プログラムのブロック機能を使用して正規のファイル</span><span class="sxs-lookup"><span data-stu-id="104f0-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="104f0-115">高</span><span class="sxs-lookup"><span data-stu-id="104f0-115">high</span></span>|<span data-ttu-id="104f0-116">1</span><span class="sxs-lookup"><span data-stu-id="104f0-116">1</span></span>|<span data-ttu-id="104f0-117">高には、強力な検出レベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="104f0-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="104f0-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="104f0-118">highPlus</span></span>|<span data-ttu-id="104f0-119">2</span><span class="sxs-lookup"><span data-stu-id="104f0-119">2</span></span>|<span data-ttu-id="104f0-120">高 + 高レベルを使用し、追加の保護手段を適用します。</span><span class="sxs-lookup"><span data-stu-id="104f0-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="104f0-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="104f0-121">zeroTolerance</span></span>|<span data-ttu-id="104f0-122">3</span><span class="sxs-lookup"><span data-stu-id="104f0-122">3</span></span>|<span data-ttu-id="104f0-123">耐は、すべての不明な実行可能ファイルをブロックします。</span><span class="sxs-lookup"><span data-stu-id="104f0-123">Zero tolerance blocks all unknown executables</span></span>|




