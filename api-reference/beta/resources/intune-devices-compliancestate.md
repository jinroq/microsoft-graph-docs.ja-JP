---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6fff27abba5bce945b1f8abd74e94e2060114b17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000019"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="13ea0-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="13ea0-103">complianceState enum type</span></span>

> <span data-ttu-id="13ea0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13ea0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13ea0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13ea0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13ea0-106">コンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="13ea0-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="13ea0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="13ea0-107">Members</span></span>
|<span data-ttu-id="13ea0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="13ea0-108">Member</span></span>|<span data-ttu-id="13ea0-109">値</span><span class="sxs-lookup"><span data-stu-id="13ea0-109">Value</span></span>|<span data-ttu-id="13ea0-110">説明</span><span class="sxs-lookup"><span data-stu-id="13ea0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ea0-111">不明</span><span class="sxs-lookup"><span data-stu-id="13ea0-111">unknown</span></span>|<span data-ttu-id="13ea0-112">.0</span><span class="sxs-lookup"><span data-stu-id="13ea0-112">0</span></span>|<span data-ttu-id="13ea0-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="13ea0-113">Unknown.</span></span>|
|<span data-ttu-id="13ea0-114">要件</span><span class="sxs-lookup"><span data-stu-id="13ea0-114">compliant</span></span>|<span data-ttu-id="13ea0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="13ea0-115">1</span></span>|<span data-ttu-id="13ea0-116">要件.</span><span class="sxs-lookup"><span data-stu-id="13ea0-116">Compliant.</span></span>|
|<span data-ttu-id="13ea0-117">互換性</span><span class="sxs-lookup"><span data-stu-id="13ea0-117">noncompliant</span></span>|<span data-ttu-id="13ea0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="13ea0-118">2</span></span>|<span data-ttu-id="13ea0-119">デバイスは非準拠で、企業リソースからブロックされます。</span><span class="sxs-lookup"><span data-stu-id="13ea0-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="13ea0-120">異なる</span><span class="sxs-lookup"><span data-stu-id="13ea0-120">conflict</span></span>|<span data-ttu-id="13ea0-121">1/3</span><span class="sxs-lookup"><span data-stu-id="13ea0-121">3</span></span>|<span data-ttu-id="13ea0-122">他のルールと競合しています。</span><span class="sxs-lookup"><span data-stu-id="13ea0-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="13ea0-123">error</span><span class="sxs-lookup"><span data-stu-id="13ea0-123">error</span></span>|<span data-ttu-id="13ea0-124">2/4</span><span class="sxs-lookup"><span data-stu-id="13ea0-124">4</span></span>|<span data-ttu-id="13ea0-125">Error。</span><span class="sxs-lookup"><span data-stu-id="13ea0-125">Error.</span></span>|
|<span data-ttu-id="13ea0-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="13ea0-126">inGracePeriod</span></span>|<span data-ttu-id="13ea0-127">254</span><span class="sxs-lookup"><span data-stu-id="13ea0-127">254</span></span>|<span data-ttu-id="13ea0-128">デバイスは準拠していないが、会社のリソースにアクセスできる</span><span class="sxs-lookup"><span data-stu-id="13ea0-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="13ea0-129">configManager</span><span class="sxs-lookup"><span data-stu-id="13ea0-129">configManager</span></span>|<span data-ttu-id="13ea0-130">255</span><span class="sxs-lookup"><span data-stu-id="13ea0-130">255</span></span>|<span data-ttu-id="13ea0-131">構成マネージャーによる管理</span><span class="sxs-lookup"><span data-stu-id="13ea0-131">Managed by Config Manager</span></span>|





