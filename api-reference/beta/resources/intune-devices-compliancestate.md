---
title: complianceState 列挙型
description: コンプライアンスの状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8c462df866b3c711bf4738c70ad4a1b0d68ceeb4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549126"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="5f9e4-103">complianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="5f9e4-103">complianceState enum type</span></span>

> <span data-ttu-id="5f9e4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f9e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f9e4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f9e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f9e4-106">コンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="5f9e4-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="5f9e4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5f9e4-107">Members</span></span>
|<span data-ttu-id="5f9e4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5f9e4-108">Member</span></span>|<span data-ttu-id="5f9e4-109">値</span><span class="sxs-lookup"><span data-stu-id="5f9e4-109">Value</span></span>|<span data-ttu-id="5f9e4-110">説明</span><span class="sxs-lookup"><span data-stu-id="5f9e4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f9e4-111">不明</span><span class="sxs-lookup"><span data-stu-id="5f9e4-111">unknown</span></span>|<span data-ttu-id="5f9e4-112">.0</span><span class="sxs-lookup"><span data-stu-id="5f9e4-112">0</span></span>|<span data-ttu-id="5f9e4-113">わかり.</span><span class="sxs-lookup"><span data-stu-id="5f9e4-113">Unknown.</span></span>|
|<span data-ttu-id="5f9e4-114">要件</span><span class="sxs-lookup"><span data-stu-id="5f9e4-114">compliant</span></span>|<span data-ttu-id="5f9e4-115">1 </span><span class="sxs-lookup"><span data-stu-id="5f9e4-115">1</span></span>|<span data-ttu-id="5f9e4-116">要件.</span><span class="sxs-lookup"><span data-stu-id="5f9e4-116">Compliant.</span></span>|
|<span data-ttu-id="5f9e4-117">互換性</span><span class="sxs-lookup"><span data-stu-id="5f9e4-117">noncompliant</span></span>|<span data-ttu-id="5f9e4-118">2 </span><span class="sxs-lookup"><span data-stu-id="5f9e4-118">2</span></span>|<span data-ttu-id="5f9e4-119">デバイスは非準拠で、企業リソースからブロックされます。</span><span class="sxs-lookup"><span data-stu-id="5f9e4-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="5f9e4-120">異なる</span><span class="sxs-lookup"><span data-stu-id="5f9e4-120">conflict</span></span>|<span data-ttu-id="5f9e4-121">3 </span><span class="sxs-lookup"><span data-stu-id="5f9e4-121">3</span></span>|<span data-ttu-id="5f9e4-122">他のルールと競合しています。</span><span class="sxs-lookup"><span data-stu-id="5f9e4-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="5f9e4-123">error</span><span class="sxs-lookup"><span data-stu-id="5f9e4-123">error</span></span>|<span data-ttu-id="5f9e4-124">4 </span><span class="sxs-lookup"><span data-stu-id="5f9e4-124">4</span></span>|<span data-ttu-id="5f9e4-125">Error。</span><span class="sxs-lookup"><span data-stu-id="5f9e4-125">Error.</span></span>|
|<span data-ttu-id="5f9e4-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="5f9e4-126">inGracePeriod</span></span>|<span data-ttu-id="5f9e4-127">254</span><span class="sxs-lookup"><span data-stu-id="5f9e4-127">254</span></span>|<span data-ttu-id="5f9e4-128">デバイスは準拠していないが、会社のリソースにアクセスできる</span><span class="sxs-lookup"><span data-stu-id="5f9e4-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="5f9e4-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="5f9e4-129">configManager</span></span>|<span data-ttu-id="5f9e4-130">255</span><span class="sxs-lookup"><span data-stu-id="5f9e4-130">255</span></span>|<span data-ttu-id="5f9e4-131">構成マネージャーによる管理</span><span class="sxs-lookup"><span data-stu-id="5f9e4-131">Managed by Config Manager</span></span>|





