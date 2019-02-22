---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29357c5248aea78ffca8af464ecf4c3af17bdbc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172927"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="262a1-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="262a1-103">complianceState enum type</span></span>

> <span data-ttu-id="262a1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="262a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="262a1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="262a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="262a1-106">コンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="262a1-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="262a1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="262a1-107">Members</span></span>
|<span data-ttu-id="262a1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="262a1-108">Member</span></span>|<span data-ttu-id="262a1-109">値</span><span class="sxs-lookup"><span data-stu-id="262a1-109">Value</span></span>|<span data-ttu-id="262a1-110">説明</span><span class="sxs-lookup"><span data-stu-id="262a1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="262a1-111">不明</span><span class="sxs-lookup"><span data-stu-id="262a1-111">unknown</span></span>|<span data-ttu-id="262a1-112">.0</span><span class="sxs-lookup"><span data-stu-id="262a1-112">0</span></span>|<span data-ttu-id="262a1-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="262a1-113">Unknown.</span></span>|
|<span data-ttu-id="262a1-114">要件</span><span class="sxs-lookup"><span data-stu-id="262a1-114">compliant</span></span>|<span data-ttu-id="262a1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="262a1-115">1</span></span>|<span data-ttu-id="262a1-116">要件.</span><span class="sxs-lookup"><span data-stu-id="262a1-116">Compliant.</span></span>|
|<span data-ttu-id="262a1-117">互換性</span><span class="sxs-lookup"><span data-stu-id="262a1-117">noncompliant</span></span>|<span data-ttu-id="262a1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="262a1-118">2</span></span>|<span data-ttu-id="262a1-119">デバイスは非準拠で、企業リソースからブロックされます。</span><span class="sxs-lookup"><span data-stu-id="262a1-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="262a1-120">異なる</span><span class="sxs-lookup"><span data-stu-id="262a1-120">conflict</span></span>|<span data-ttu-id="262a1-121">1/3</span><span class="sxs-lookup"><span data-stu-id="262a1-121">3</span></span>|<span data-ttu-id="262a1-122">他のルールと競合しています。</span><span class="sxs-lookup"><span data-stu-id="262a1-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="262a1-123">エラー</span><span class="sxs-lookup"><span data-stu-id="262a1-123">error</span></span>|<span data-ttu-id="262a1-124">2/4</span><span class="sxs-lookup"><span data-stu-id="262a1-124">4</span></span>|<span data-ttu-id="262a1-125">エラー。</span><span class="sxs-lookup"><span data-stu-id="262a1-125">Error.</span></span>|
|<span data-ttu-id="262a1-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="262a1-126">inGracePeriod</span></span>|<span data-ttu-id="262a1-127">254</span><span class="sxs-lookup"><span data-stu-id="262a1-127">254</span></span>|<span data-ttu-id="262a1-128">デバイスは準拠していないが、会社のリソースにアクセスできる</span><span class="sxs-lookup"><span data-stu-id="262a1-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="262a1-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="262a1-129">configManager</span></span>|<span data-ttu-id="262a1-130">255</span><span class="sxs-lookup"><span data-stu-id="262a1-130">255</span></span>|<span data-ttu-id="262a1-131">構成マネージャーによる管理</span><span class="sxs-lookup"><span data-stu-id="262a1-131">Managed by Config Manager</span></span>|




