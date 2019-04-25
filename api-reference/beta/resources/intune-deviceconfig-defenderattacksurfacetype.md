---
title: defenderAttackSurfaceType 列挙型
description: Defender 攻撃面の削減ルールの可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29610eca9dbb157a5ce4d51bcb67fa479814d17d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549294"
---
# <a name="defenderattacksurfacetype-enum-type"></a><span data-ttu-id="66c28-103">defenderAttackSurfaceType 列挙型</span><span class="sxs-lookup"><span data-stu-id="66c28-103">defenderAttackSurfaceType enum type</span></span>

> <span data-ttu-id="66c28-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66c28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66c28-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66c28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66c28-106">Defender 攻撃面の削減ルールの可能な値</span><span class="sxs-lookup"><span data-stu-id="66c28-106">Possible values of Defender Attack Surface Reduction Rules</span></span>

## <a name="members"></a><span data-ttu-id="66c28-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="66c28-107">Members</span></span>
|<span data-ttu-id="66c28-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="66c28-108">Member</span></span>|<span data-ttu-id="66c28-109">値</span><span class="sxs-lookup"><span data-stu-id="66c28-109">Value</span></span>|<span data-ttu-id="66c28-110">説明</span><span class="sxs-lookup"><span data-stu-id="66c28-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66c28-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="66c28-111">userDefined</span></span>|<span data-ttu-id="66c28-112">.0</span><span class="sxs-lookup"><span data-stu-id="66c28-112">0</span></span>|<span data-ttu-id="66c28-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="66c28-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="66c28-114">拒否</span><span class="sxs-lookup"><span data-stu-id="66c28-114">block</span></span>|<span data-ttu-id="66c28-115">1 </span><span class="sxs-lookup"><span data-stu-id="66c28-115">1</span></span>|<span data-ttu-id="66c28-116">機能をブロックする。</span><span class="sxs-lookup"><span data-stu-id="66c28-116">Block functionality.</span></span>|
|<span data-ttu-id="66c28-117">auditmode</span><span class="sxs-lookup"><span data-stu-id="66c28-117">auditMode</span></span>|<span data-ttu-id="66c28-118">2 </span><span class="sxs-lookup"><span data-stu-id="66c28-118">2</span></span>|<span data-ttu-id="66c28-119">機能は変更されませんが、ログは生成されません。</span><span class="sxs-lookup"><span data-stu-id="66c28-119">Does not change functionality but generate logs.</span></span>|





