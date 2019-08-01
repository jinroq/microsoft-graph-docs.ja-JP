---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 20890001aee15a56d5338964b931047033cf4a72
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030885"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="de360-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="de360-103">complianceState enum type</span></span>

> <span data-ttu-id="de360-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="de360-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de360-105">コンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="de360-105">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="de360-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="de360-106">Members</span></span>
|<span data-ttu-id="de360-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="de360-107">Member</span></span>|<span data-ttu-id="de360-108">値</span><span class="sxs-lookup"><span data-stu-id="de360-108">Value</span></span>|<span data-ttu-id="de360-109">説明</span><span class="sxs-lookup"><span data-stu-id="de360-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de360-110">不明</span><span class="sxs-lookup"><span data-stu-id="de360-110">unknown</span></span>|<span data-ttu-id="de360-111">.0</span><span class="sxs-lookup"><span data-stu-id="de360-111">0</span></span>|<span data-ttu-id="de360-112">わかり.</span><span class="sxs-lookup"><span data-stu-id="de360-112">Unknown.</span></span>|
|<span data-ttu-id="de360-113">要件</span><span class="sxs-lookup"><span data-stu-id="de360-113">compliant</span></span>|<span data-ttu-id="de360-114">1-d</span><span class="sxs-lookup"><span data-stu-id="de360-114">1</span></span>|<span data-ttu-id="de360-115">要件.</span><span class="sxs-lookup"><span data-stu-id="de360-115">Compliant.</span></span>|
|<span data-ttu-id="de360-116">互換性</span><span class="sxs-lookup"><span data-stu-id="de360-116">noncompliant</span></span>|<span data-ttu-id="de360-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="de360-117">2</span></span>|<span data-ttu-id="de360-118">デバイスは非準拠で、企業リソースからブロックされます。</span><span class="sxs-lookup"><span data-stu-id="de360-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="de360-119">異なる</span><span class="sxs-lookup"><span data-stu-id="de360-119">conflict</span></span>|<span data-ttu-id="de360-120">1/3</span><span class="sxs-lookup"><span data-stu-id="de360-120">3</span></span>|<span data-ttu-id="de360-121">他のルールと競合しています。</span><span class="sxs-lookup"><span data-stu-id="de360-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="de360-122">error</span><span class="sxs-lookup"><span data-stu-id="de360-122">error</span></span>|<span data-ttu-id="de360-123">2/4</span><span class="sxs-lookup"><span data-stu-id="de360-123">4</span></span>|<span data-ttu-id="de360-124">Error。</span><span class="sxs-lookup"><span data-stu-id="de360-124">Error.</span></span>|
|<span data-ttu-id="de360-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="de360-125">inGracePeriod</span></span>|<span data-ttu-id="de360-126">254</span><span class="sxs-lookup"><span data-stu-id="de360-126">254</span></span>|<span data-ttu-id="de360-127">デバイスは準拠していないが、会社のリソースにアクセスできる</span><span class="sxs-lookup"><span data-stu-id="de360-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="de360-128">configManager</span><span class="sxs-lookup"><span data-stu-id="de360-128">configManager</span></span>|<span data-ttu-id="de360-129">255</span><span class="sxs-lookup"><span data-stu-id="de360-129">255</span></span>|<span data-ttu-id="de360-130">構成マネージャーによる管理</span><span class="sxs-lookup"><span data-stu-id="de360-130">Managed by Config Manager</span></span>|



