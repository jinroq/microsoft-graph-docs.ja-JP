---
title: vpnTrafficRuleAppType 列挙型
description: VPN トラフィックの規則が関連付けられているアプリケーションの種類を示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 061cb5701830939576f5b9a649c73b4d44eada18
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396022"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="55fbd-103">vpnTrafficRuleAppType 列挙型</span><span class="sxs-lookup"><span data-stu-id="55fbd-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="55fbd-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="55fbd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="55fbd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55fbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55fbd-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="55fbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55fbd-107">VPN トラフィックの規則が関連付けられているアプリケーションの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="55fbd-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="55fbd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="55fbd-108">Members</span></span>
|<span data-ttu-id="55fbd-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="55fbd-109">Member</span></span>|<span data-ttu-id="55fbd-110">値</span><span class="sxs-lookup"><span data-stu-id="55fbd-110">Value</span></span>|<span data-ttu-id="55fbd-111">説明</span><span class="sxs-lookup"><span data-stu-id="55fbd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55fbd-112">none</span><span class="sxs-lookup"><span data-stu-id="55fbd-112">none</span></span>|<span data-ttu-id="55fbd-113">0</span><span class="sxs-lookup"><span data-stu-id="55fbd-113">0</span></span>|<span data-ttu-id="55fbd-114">トラフィックの規則は、アプリケーションに関連付けられているではありません。</span><span class="sxs-lookup"><span data-stu-id="55fbd-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="55fbd-115">デスクトップ</span><span class="sxs-lookup"><span data-stu-id="55fbd-115">desktop</span></span>|<span data-ttu-id="55fbd-116">1</span><span class="sxs-lookup"><span data-stu-id="55fbd-116">1</span></span>|<span data-ttu-id="55fbd-117">トラフィックの規則では、デスクトップ アプリケーションに関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="55fbd-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="55fbd-118">ユニバーサル</span><span class="sxs-lookup"><span data-stu-id="55fbd-118">universal</span></span>|<span data-ttu-id="55fbd-119">2</span><span class="sxs-lookup"><span data-stu-id="55fbd-119">2</span></span>|<span data-ttu-id="55fbd-120">トラフィックの規則では、汎用のアプリケーションに関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="55fbd-120">The traffic rule is associated with a Universal app.</span></span>|




