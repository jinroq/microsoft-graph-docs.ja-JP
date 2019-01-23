---
title: complianceState 列挙型
description: コンプライアンス状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 04f77da451970a302dbf249e8820aa5a2a8f0ebc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392739"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="af9f2-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="af9f2-103">complianceState enum type</span></span>

> <span data-ttu-id="af9f2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="af9f2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af9f2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af9f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af9f2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af9f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af9f2-107">コンプライアンス状態です。</span><span class="sxs-lookup"><span data-stu-id="af9f2-107">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="af9f2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="af9f2-108">Members</span></span>
|<span data-ttu-id="af9f2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="af9f2-109">Member</span></span>|<span data-ttu-id="af9f2-110">値</span><span class="sxs-lookup"><span data-stu-id="af9f2-110">Value</span></span>|<span data-ttu-id="af9f2-111">説明</span><span class="sxs-lookup"><span data-stu-id="af9f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af9f2-112">不明</span><span class="sxs-lookup"><span data-stu-id="af9f2-112">unknown</span></span>|<span data-ttu-id="af9f2-113">0</span><span class="sxs-lookup"><span data-stu-id="af9f2-113">0</span></span>|<span data-ttu-id="af9f2-114">不明。</span><span class="sxs-lookup"><span data-stu-id="af9f2-114">Unknown.</span></span>|
|<span data-ttu-id="af9f2-115">準拠</span><span class="sxs-lookup"><span data-stu-id="af9f2-115">compliant</span></span>|<span data-ttu-id="af9f2-116">1</span><span class="sxs-lookup"><span data-stu-id="af9f2-116">1</span></span>|<span data-ttu-id="af9f2-117">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="af9f2-117">Compliant.</span></span>|
|<span data-ttu-id="af9f2-118">準拠していません。</span><span class="sxs-lookup"><span data-stu-id="af9f2-118">noncompliant</span></span>|<span data-ttu-id="af9f2-119">2</span><span class="sxs-lookup"><span data-stu-id="af9f2-119">2</span></span>|<span data-ttu-id="af9f2-120">デバイスは非準拠、企業のリソースがブロックされました。</span><span class="sxs-lookup"><span data-stu-id="af9f2-120">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="af9f2-121">競合</span><span class="sxs-lookup"><span data-stu-id="af9f2-121">conflict</span></span>|<span data-ttu-id="af9f2-122">3</span><span class="sxs-lookup"><span data-stu-id="af9f2-122">3</span></span>|<span data-ttu-id="af9f2-123">その他の規則と競合しています。</span><span class="sxs-lookup"><span data-stu-id="af9f2-123">Conflict with other rules.</span></span>|
|<span data-ttu-id="af9f2-124">エラー</span><span class="sxs-lookup"><span data-stu-id="af9f2-124">error</span></span>|<span data-ttu-id="af9f2-125">4</span><span class="sxs-lookup"><span data-stu-id="af9f2-125">4</span></span>|<span data-ttu-id="af9f2-126">エラー。</span><span class="sxs-lookup"><span data-stu-id="af9f2-126">Error.</span></span>|
|<span data-ttu-id="af9f2-127">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="af9f2-127">inGracePeriod</span></span>|<span data-ttu-id="af9f2-128">254</span><span class="sxs-lookup"><span data-stu-id="af9f2-128">254</span></span>|<span data-ttu-id="af9f2-129">デバイスは非準拠ですが、社内リソースへのアクセスにはまだ</span><span class="sxs-lookup"><span data-stu-id="af9f2-129">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="af9f2-130">configManager</span><span class="sxs-lookup"><span data-stu-id="af9f2-130">configManager</span></span>|<span data-ttu-id="af9f2-131">255</span><span class="sxs-lookup"><span data-stu-id="af9f2-131">255</span></span>|<span data-ttu-id="af9f2-132">構成マネージャーによって管理されます。</span><span class="sxs-lookup"><span data-stu-id="af9f2-132">Managed by Config Manager</span></span>|




