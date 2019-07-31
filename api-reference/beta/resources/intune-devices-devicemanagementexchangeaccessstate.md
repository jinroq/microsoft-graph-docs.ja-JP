---
title: deviceManagementExchangeAccessState 列挙型
description: デバイスの Exchange アクセス状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 26f75ccd2957d7cc9db9b05bb48f4a9eacc36a17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999900"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="bbf80-103">deviceManagementExchangeAccessState 列挙型</span><span class="sxs-lookup"><span data-stu-id="bbf80-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="bbf80-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbf80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbf80-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bbf80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbf80-106">デバイスの Exchange アクセス状態。</span><span class="sxs-lookup"><span data-stu-id="bbf80-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="bbf80-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bbf80-107">Members</span></span>
|<span data-ttu-id="bbf80-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bbf80-108">Member</span></span>|<span data-ttu-id="bbf80-109">値</span><span class="sxs-lookup"><span data-stu-id="bbf80-109">Value</span></span>|<span data-ttu-id="bbf80-110">説明</span><span class="sxs-lookup"><span data-stu-id="bbf80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbf80-111">none</span><span class="sxs-lookup"><span data-stu-id="bbf80-111">none</span></span>|<span data-ttu-id="bbf80-112">.0</span><span class="sxs-lookup"><span data-stu-id="bbf80-112">0</span></span>|<span data-ttu-id="bbf80-113">Exchange から検出されたアクセス状態なし</span><span class="sxs-lookup"><span data-stu-id="bbf80-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="bbf80-114">不明</span><span class="sxs-lookup"><span data-stu-id="bbf80-114">unknown</span></span>|<span data-ttu-id="bbf80-115">1-d</span><span class="sxs-lookup"><span data-stu-id="bbf80-115">1</span></span>|<span data-ttu-id="bbf80-116">Exchange へのデバイスアクセス状態が不明です</span><span class="sxs-lookup"><span data-stu-id="bbf80-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="bbf80-117">れる</span><span class="sxs-lookup"><span data-stu-id="bbf80-117">allowed</span></span>|<span data-ttu-id="bbf80-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="bbf80-118">2</span></span>|<span data-ttu-id="bbf80-119">デバイスが Exchange にアクセスできる</span><span class="sxs-lookup"><span data-stu-id="bbf80-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="bbf80-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="bbf80-120">blocked</span></span>|<span data-ttu-id="bbf80-121">1/3</span><span class="sxs-lookup"><span data-stu-id="bbf80-121">3</span></span>|<span data-ttu-id="bbf80-122">Exchange でデバイスがブロックされている</span><span class="sxs-lookup"><span data-stu-id="bbf80-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="bbf80-123">隔離</span><span class="sxs-lookup"><span data-stu-id="bbf80-123">quarantined</span></span>|<span data-ttu-id="bbf80-124">2/4</span><span class="sxs-lookup"><span data-stu-id="bbf80-124">4</span></span>|<span data-ttu-id="bbf80-125">Exchange でのデバイスの検疫</span><span class="sxs-lookup"><span data-stu-id="bbf80-125">Device is Quarantined in Exchange</span></span>|





