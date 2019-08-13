---
title: powerActionType 列挙型
description: 電源アクションの種類
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 47ab4ba877f5563ff57d20eadde42f241713b311
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371534"
---
# <a name="poweractiontype-enum-type"></a><span data-ttu-id="a1497-103">powerActionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a1497-103">powerActionType enum type</span></span>

> <span data-ttu-id="a1497-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1497-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1497-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1497-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1497-106">電源アクションの種類</span><span class="sxs-lookup"><span data-stu-id="a1497-106">Power action types</span></span>

## <a name="members"></a><span data-ttu-id="a1497-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1497-107">Members</span></span>
|<span data-ttu-id="a1497-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1497-108">Member</span></span>|<span data-ttu-id="a1497-109">値</span><span class="sxs-lookup"><span data-stu-id="a1497-109">Value</span></span>|<span data-ttu-id="a1497-110">説明</span><span class="sxs-lookup"><span data-stu-id="a1497-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1497-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a1497-111">notConfigured</span></span>|<span data-ttu-id="a1497-112">.0</span><span class="sxs-lookup"><span data-stu-id="a1497-112">0</span></span>|<span data-ttu-id="a1497-113">未構成</span><span class="sxs-lookup"><span data-stu-id="a1497-113">Not configured</span></span>|
|<span data-ttu-id="a1497-114">noAction</span><span class="sxs-lookup"><span data-stu-id="a1497-114">noAction</span></span>|<span data-ttu-id="a1497-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a1497-115">1</span></span>|<span data-ttu-id="a1497-116">アクションなし</span><span class="sxs-lookup"><span data-stu-id="a1497-116">No action</span></span>|
|<span data-ttu-id="a1497-117">デバイス</span><span class="sxs-lookup"><span data-stu-id="a1497-117">sleep</span></span>|<span data-ttu-id="a1497-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a1497-118">2</span></span>|<span data-ttu-id="a1497-119">デバイスをスリープ状態にする</span><span class="sxs-lookup"><span data-stu-id="a1497-119">Put device in sleep state</span></span>|
|<span data-ttu-id="a1497-120">休止</span><span class="sxs-lookup"><span data-stu-id="a1497-120">hibernate</span></span>|<span data-ttu-id="a1497-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a1497-121">3</span></span>|<span data-ttu-id="a1497-122">デバイスを休止状態にする</span><span class="sxs-lookup"><span data-stu-id="a1497-122">Put device in hibernate state</span></span>|
|<span data-ttu-id="a1497-123">シャット</span><span class="sxs-lookup"><span data-stu-id="a1497-123">shutdown</span></span>|<span data-ttu-id="a1497-124">2/4</span><span class="sxs-lookup"><span data-stu-id="a1497-124">4</span></span>|<span data-ttu-id="a1497-125">シャットダウンデバイス</span><span class="sxs-lookup"><span data-stu-id="a1497-125">Shutdown device</span></span>|



