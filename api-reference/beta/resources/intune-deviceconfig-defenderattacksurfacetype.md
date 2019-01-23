---
title: defenderAttackSurfaceType 列挙型
description: Defender 攻撃面の削減ルールで使用できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b8972fff25cb75d3cef1848985db0292753959fa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399662"
---
# <a name="defenderattacksurfacetype-enum-type"></a><span data-ttu-id="1c067-103">defenderAttackSurfaceType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1c067-103">defenderAttackSurfaceType enum type</span></span>

> <span data-ttu-id="1c067-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1c067-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1c067-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c067-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c067-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1c067-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c067-107">Defender 攻撃面の削減ルールで使用できる値</span><span class="sxs-lookup"><span data-stu-id="1c067-107">Possible values of Defender Attack Surface Reduction Rules</span></span>

## <a name="members"></a><span data-ttu-id="1c067-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1c067-108">Members</span></span>
|<span data-ttu-id="1c067-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1c067-109">Member</span></span>|<span data-ttu-id="1c067-110">値</span><span class="sxs-lookup"><span data-stu-id="1c067-110">Value</span></span>|<span data-ttu-id="1c067-111">説明</span><span class="sxs-lookup"><span data-stu-id="1c067-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c067-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="1c067-112">userDefined</span></span>|<span data-ttu-id="1c067-113">0</span><span class="sxs-lookup"><span data-stu-id="1c067-113">0</span></span>|<span data-ttu-id="1c067-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="1c067-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="1c067-115">ブロック</span><span class="sxs-lookup"><span data-stu-id="1c067-115">block</span></span>|<span data-ttu-id="1c067-116">1</span><span class="sxs-lookup"><span data-stu-id="1c067-116">1</span></span>|<span data-ttu-id="1c067-117">機能をブロックします。</span><span class="sxs-lookup"><span data-stu-id="1c067-117">Block functionality.</span></span>|
|<span data-ttu-id="1c067-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="1c067-118">auditMode</span></span>|<span data-ttu-id="1c067-119">2</span><span class="sxs-lookup"><span data-stu-id="1c067-119">2</span></span>|<span data-ttu-id="1c067-120">機能は変更されませんが、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="1c067-120">Does not change functionality but generate logs.</span></span>|




