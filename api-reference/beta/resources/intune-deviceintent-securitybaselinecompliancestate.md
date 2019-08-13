---
title: securityBaselineComplianceState 列挙型
description: セキュリティベースラインコンプライアンスの状態
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6a287ede8651b3466acdd4ebe229eb1a0f84810d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319378"
---
# <a name="securitybaselinecompliancestate-enum-type"></a><span data-ttu-id="6ce88-103">securityBaselineComplianceState 列挙型</span><span class="sxs-lookup"><span data-stu-id="6ce88-103">securityBaselineComplianceState enum type</span></span>

> <span data-ttu-id="6ce88-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ce88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ce88-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ce88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ce88-106">セキュリティベースラインコンプライアンスの状態</span><span class="sxs-lookup"><span data-stu-id="6ce88-106">Security Baseline Compliance State</span></span>

## <a name="members"></a><span data-ttu-id="6ce88-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6ce88-107">Members</span></span>
|<span data-ttu-id="6ce88-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6ce88-108">Member</span></span>|<span data-ttu-id="6ce88-109">値</span><span class="sxs-lookup"><span data-stu-id="6ce88-109">Value</span></span>|<span data-ttu-id="6ce88-110">説明</span><span class="sxs-lookup"><span data-stu-id="6ce88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce88-111">不明</span><span class="sxs-lookup"><span data-stu-id="6ce88-111">unknown</span></span>|<span data-ttu-id="6ce88-112">.0</span><span class="sxs-lookup"><span data-stu-id="6ce88-112">0</span></span>|<span data-ttu-id="6ce88-113">不明な状態</span><span class="sxs-lookup"><span data-stu-id="6ce88-113">Unknown state</span></span>|
|<span data-ttu-id="6ce88-114">な</span><span class="sxs-lookup"><span data-stu-id="6ce88-114">secure</span></span>|<span data-ttu-id="6ce88-115">1-d</span><span class="sxs-lookup"><span data-stu-id="6ce88-115">1</span></span>|<span data-ttu-id="6ce88-116">セキュリティで保護された状態</span><span class="sxs-lookup"><span data-stu-id="6ce88-116">Secure state</span></span>|
|<span data-ttu-id="6ce88-117">notApplicable</span><span class="sxs-lookup"><span data-stu-id="6ce88-117">notApplicable</span></span>|<span data-ttu-id="6ce88-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6ce88-118">2</span></span>|<span data-ttu-id="6ce88-119">該当なしの状態</span><span class="sxs-lookup"><span data-stu-id="6ce88-119">Not applicable state</span></span>|
|<span data-ttu-id="6ce88-120">notSecure</span><span class="sxs-lookup"><span data-stu-id="6ce88-120">notSecure</span></span>|<span data-ttu-id="6ce88-121">1/3</span><span class="sxs-lookup"><span data-stu-id="6ce88-121">3</span></span>|<span data-ttu-id="6ce88-122">セキュリティで保護されていない状態</span><span class="sxs-lookup"><span data-stu-id="6ce88-122">Not secure state</span></span>|
|<span data-ttu-id="6ce88-123">error</span><span class="sxs-lookup"><span data-stu-id="6ce88-123">error</span></span>|<span data-ttu-id="6ce88-124">2/4</span><span class="sxs-lookup"><span data-stu-id="6ce88-124">4</span></span>|<span data-ttu-id="6ce88-125">エラー状態</span><span class="sxs-lookup"><span data-stu-id="6ce88-125">Error state</span></span>|
|<span data-ttu-id="6ce88-126">異なる</span><span class="sxs-lookup"><span data-stu-id="6ce88-126">conflict</span></span>|<span data-ttu-id="6ce88-127">5</span><span class="sxs-lookup"><span data-stu-id="6ce88-127">5</span></span>|<span data-ttu-id="6ce88-128">競合状態</span><span class="sxs-lookup"><span data-stu-id="6ce88-128">Conflict state</span></span>|



