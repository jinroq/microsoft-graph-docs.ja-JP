---
title: defendercloudblockleveltype 列挙型
description: クラウドブロックレベルの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de81e42827f7c153fc81e7fc19d85e54cb780bfa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575185"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="8f113-103">defendercloudblockleveltype 列挙型</span><span class="sxs-lookup"><span data-stu-id="8f113-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="8f113-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f113-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f113-105">クラウドブロックレベルの可能な値</span><span class="sxs-lookup"><span data-stu-id="8f113-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="8f113-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="8f113-106">Members</span></span>
|<span data-ttu-id="8f113-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8f113-107">Member</span></span>|<span data-ttu-id="8f113-108">値</span><span class="sxs-lookup"><span data-stu-id="8f113-108">Value</span></span>|<span data-ttu-id="8f113-109">説明</span><span class="sxs-lookup"><span data-stu-id="8f113-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f113-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8f113-110">notConfigured</span></span>|<span data-ttu-id="8f113-111">.0</span><span class="sxs-lookup"><span data-stu-id="8f113-111">0</span></span>|<span data-ttu-id="8f113-112">既定値は、Windows Defender ウイルス対策の既定のブロックレベルを使用し、正当なファイルを検出するリスクを増やさずに、強力な検出を提供します。</span><span class="sxs-lookup"><span data-stu-id="8f113-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="8f113-113">高額</span><span class="sxs-lookup"><span data-stu-id="8f113-113">high</span></span>|<span data-ttu-id="8f113-114">1 </span><span class="sxs-lookup"><span data-stu-id="8f113-114">1</span></span>|<span data-ttu-id="8f113-115">High は、強力なレベルの検出を適用します。</span><span class="sxs-lookup"><span data-stu-id="8f113-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="8f113-116">highplus</span><span class="sxs-lookup"><span data-stu-id="8f113-116">highPlus</span></span>|<span data-ttu-id="8f113-117">2 </span><span class="sxs-lookup"><span data-stu-id="8f113-117">2</span></span>|<span data-ttu-id="8f113-118">高 + は高レベルを使用し、追加の保護対策を適用します。</span><span class="sxs-lookup"><span data-stu-id="8f113-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="8f113-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="8f113-119">zeroTolerance</span></span>|<span data-ttu-id="8f113-120">3 </span><span class="sxs-lookup"><span data-stu-id="8f113-120">3</span></span>|<span data-ttu-id="8f113-121">ゼロトレランスによってすべての不明な実行可能ファイルがブロック</span><span class="sxs-lookup"><span data-stu-id="8f113-121">Zero tolerance blocks all unknown executables</span></span>|



