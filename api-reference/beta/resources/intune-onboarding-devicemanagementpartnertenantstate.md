---
title: deviceManagementPartnerTenantState 列挙型
description: このテナントのパートナーの状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a7c2c7e36d920a7f8ab08be75324983f583174b2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992970"
---
# <a name="devicemanagementpartnertenantstate-enum-type"></a><span data-ttu-id="ce61c-103">deviceManagementPartnerTenantState 列挙型</span><span class="sxs-lookup"><span data-stu-id="ce61c-103">deviceManagementPartnerTenantState enum type</span></span>

> <span data-ttu-id="ce61c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce61c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce61c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce61c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce61c-106">このテナントのパートナーの状態。</span><span class="sxs-lookup"><span data-stu-id="ce61c-106">Partner state of this tenant.</span></span>

## <a name="members"></a><span data-ttu-id="ce61c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ce61c-107">Members</span></span>
|<span data-ttu-id="ce61c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ce61c-108">Member</span></span>|<span data-ttu-id="ce61c-109">値</span><span class="sxs-lookup"><span data-stu-id="ce61c-109">Value</span></span>|<span data-ttu-id="ce61c-110">説明</span><span class="sxs-lookup"><span data-stu-id="ce61c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce61c-111">不明</span><span class="sxs-lookup"><span data-stu-id="ce61c-111">unknown</span></span>|<span data-ttu-id="ce61c-112">.0</span><span class="sxs-lookup"><span data-stu-id="ce61c-112">0</span></span>|<span data-ttu-id="ce61c-113">パートナーの状態が不明です。</span><span class="sxs-lookup"><span data-stu-id="ce61c-113">Partner state is unknown.</span></span>|
|<span data-ttu-id="ce61c-114">無効</span><span class="sxs-lookup"><span data-stu-id="ce61c-114">unavailable</span></span>|<span data-ttu-id="ce61c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ce61c-115">1</span></span>|<span data-ttu-id="ce61c-116">パートナーは利用できません。</span><span class="sxs-lookup"><span data-stu-id="ce61c-116">Partner is unavailable.</span></span>|
|<span data-ttu-id="ce61c-117">enabled</span><span class="sxs-lookup"><span data-stu-id="ce61c-117">enabled</span></span>|<span data-ttu-id="ce61c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ce61c-118">2</span></span>|<span data-ttu-id="ce61c-119">パートナーが有効になっている。</span><span class="sxs-lookup"><span data-stu-id="ce61c-119">Partner is enabled.</span></span>|
|<span data-ttu-id="ce61c-120">停止</span><span class="sxs-lookup"><span data-stu-id="ce61c-120">terminated</span></span>|<span data-ttu-id="ce61c-121">1/3</span><span class="sxs-lookup"><span data-stu-id="ce61c-121">3</span></span>|<span data-ttu-id="ce61c-122">パートナー接続が終了します。</span><span class="sxs-lookup"><span data-stu-id="ce61c-122">Partner connection is terminated.</span></span>|
|<span data-ttu-id="ce61c-123">拒否</span><span class="sxs-lookup"><span data-stu-id="ce61c-123">rejected</span></span>|<span data-ttu-id="ce61c-124">2/4</span><span class="sxs-lookup"><span data-stu-id="ce61c-124">4</span></span>|<span data-ttu-id="ce61c-125">パートナーメッセージは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="ce61c-125">Partner messages are rejected.</span></span>|
|<span data-ttu-id="ce61c-126">なかっ</span><span class="sxs-lookup"><span data-stu-id="ce61c-126">unresponsive</span></span>|<span data-ttu-id="ce61c-127">5</span><span class="sxs-lookup"><span data-stu-id="ce61c-127">5</span></span>|<span data-ttu-id="ce61c-128">パートナーが応答していません。</span><span class="sxs-lookup"><span data-stu-id="ce61c-128">Partner is unresponsive.</span></span>|





