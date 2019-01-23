---
title: adminConsentState 列挙型
description: 管理者の承認の状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be144dae700c1555a3641f821402e90c58c1673c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421894"
---
# <a name="adminconsentstate-enum-type"></a><span data-ttu-id="40363-103">adminConsentState 列挙型</span><span class="sxs-lookup"><span data-stu-id="40363-103">adminConsentState enum type</span></span>

> <span data-ttu-id="40363-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="40363-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40363-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="40363-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40363-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="40363-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40363-107">管理者の承認の状態です。</span><span class="sxs-lookup"><span data-stu-id="40363-107">Admin consent state.</span></span>

## <a name="members"></a><span data-ttu-id="40363-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="40363-108">Members</span></span>
|<span data-ttu-id="40363-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="40363-109">Member</span></span>|<span data-ttu-id="40363-110">値</span><span class="sxs-lookup"><span data-stu-id="40363-110">Value</span></span>|<span data-ttu-id="40363-111">説明</span><span class="sxs-lookup"><span data-stu-id="40363-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40363-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="40363-112">notConfigured</span></span>|<span data-ttu-id="40363-113">0</span><span class="sxs-lookup"><span data-stu-id="40363-113">0</span></span>|<span data-ttu-id="40363-114">管理項目の構成されていません。</span><span class="sxs-lookup"><span data-stu-id="40363-114">Admin did not configure the item</span></span>|
|<span data-ttu-id="40363-115">付与</span><span class="sxs-lookup"><span data-stu-id="40363-115">granted</span></span>|<span data-ttu-id="40363-116">1</span><span class="sxs-lookup"><span data-stu-id="40363-116">1</span></span>|<span data-ttu-id="40363-117">管理の項目を与えられます。</span><span class="sxs-lookup"><span data-stu-id="40363-117">Admin granted item</span></span>|
|<span data-ttu-id="40363-118">notGranted</span><span class="sxs-lookup"><span data-stu-id="40363-118">notGranted</span></span>|<span data-ttu-id="40363-119">2</span><span class="sxs-lookup"><span data-stu-id="40363-119">2</span></span>|<span data-ttu-id="40363-120">Deos の管理項目を付与します。</span><span class="sxs-lookup"><span data-stu-id="40363-120">Admin deos not grant item</span></span>|




