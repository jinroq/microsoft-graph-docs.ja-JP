---
title: deviceManagementPartnerTenantState 列挙型
description: このテナントのパートナーの状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 91a7aaf37486742fead121f80c3dff457cef8d49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010722"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="daa97-103">deviceManagementPartnerTenantState 列挙型</span><span class="sxs-lookup"><span data-stu-id="daa97-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="daa97-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="daa97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daa97-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="daa97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daa97-106">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="daa97-106">Partner state of this tenant.</span></span>

## <a name="members"></a><span data-ttu-id="daa97-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="daa97-107">Members</span></span>
|<span data-ttu-id="daa97-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="daa97-108">Member</span></span>|<span data-ttu-id="daa97-109">値</span><span class="sxs-lookup"><span data-stu-id="daa97-109">Value</span></span>|<span data-ttu-id="daa97-110">説明</span><span class="sxs-lookup"><span data-stu-id="daa97-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daa97-111">不明</span><span class="sxs-lookup"><span data-stu-id="daa97-111">unknown</span></span>|<span data-ttu-id="daa97-112">.0</span><span class="sxs-lookup"><span data-stu-id="daa97-112">0</span></span>|<span data-ttu-id="daa97-113">パートナーの状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="daa97-113">Partner state is unknown.</span></span>|
|<span data-ttu-id="daa97-114">無効</span><span class="sxs-lookup"><span data-stu-id="daa97-114">unavailable</span></span>|<span data-ttu-id="daa97-115">1-d</span><span class="sxs-lookup"><span data-stu-id="daa97-115">1</span></span>|<span data-ttu-id="daa97-116">パートナーは利用できません。</span><span class="sxs-lookup"><span data-stu-id="daa97-116">Partner is unavailable.</span></span>|
|<span data-ttu-id="daa97-117">enabled</span><span class="sxs-lookup"><span data-stu-id="daa97-117">enabled</span></span>|<span data-ttu-id="daa97-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="daa97-118">2</span></span>|<span data-ttu-id="daa97-119">パートナーが有効になっている。</span><span class="sxs-lookup"><span data-stu-id="daa97-119">Partner is enabled.</span></span>|
|<span data-ttu-id="daa97-120">停止</span><span class="sxs-lookup"><span data-stu-id="daa97-120">terminated</span></span>|<span data-ttu-id="daa97-121">1/3</span><span class="sxs-lookup"><span data-stu-id="daa97-121">3</span></span>|<span data-ttu-id="daa97-122">パートナー接続が終了します。</span><span class="sxs-lookup"><span data-stu-id="daa97-122">Partner connection is terminated.</span></span>|
|<span data-ttu-id="daa97-123">拒否</span><span class="sxs-lookup"><span data-stu-id="daa97-123">rejected</span></span>|<span data-ttu-id="daa97-124">2/4</span><span class="sxs-lookup"><span data-stu-id="daa97-124">4</span></span>|<span data-ttu-id="daa97-125">パートナーメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="daa97-125">Partner messages are rejected.</span></span>|
|<span data-ttu-id="daa97-126">なかっ</span><span class="sxs-lookup"><span data-stu-id="daa97-126">unresponsive</span></span>|<span data-ttu-id="daa97-127">5</span><span class="sxs-lookup"><span data-stu-id="daa97-127">5</span></span>|<span data-ttu-id="daa97-128">パートナーが応答していません。</span><span class="sxs-lookup"><span data-stu-id="daa97-128">Partner is unresponsive.</span></span>|





