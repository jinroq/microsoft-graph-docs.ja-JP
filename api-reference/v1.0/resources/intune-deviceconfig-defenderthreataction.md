---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0195176f322230b3164856575880b9dadc24bce0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031781"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="f8951-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="f8951-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="f8951-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f8951-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8951-105">検出されたマルウェアの脅威を処理する Defender の既定のアクション。</span><span class="sxs-lookup"><span data-stu-id="f8951-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="f8951-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8951-106">Members</span></span>
|<span data-ttu-id="f8951-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8951-107">Member</span></span>|<span data-ttu-id="f8951-108">値</span><span class="sxs-lookup"><span data-stu-id="f8951-108">Value</span></span>|<span data-ttu-id="f8951-109">説明</span><span class="sxs-lookup"><span data-stu-id="f8951-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8951-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f8951-110">deviceDefault</span></span>|<span data-ttu-id="f8951-111">.0</span><span class="sxs-lookup"><span data-stu-id="f8951-111">0</span></span>|<span data-ttu-id="f8951-112">更新定義に基づいてアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="f8951-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="f8951-113">汚れ</span><span class="sxs-lookup"><span data-stu-id="f8951-113">clean</span></span>|<span data-ttu-id="f8951-114">1-d</span><span class="sxs-lookup"><span data-stu-id="f8951-114">1</span></span>|<span data-ttu-id="f8951-115">検出された脅威を除去します。</span><span class="sxs-lookup"><span data-stu-id="f8951-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="f8951-116">済み</span><span class="sxs-lookup"><span data-stu-id="f8951-116">quarantine</span></span>|<span data-ttu-id="f8951-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f8951-117">2</span></span>|<span data-ttu-id="f8951-118">検出された脅威を検疫します。</span><span class="sxs-lookup"><span data-stu-id="f8951-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="f8951-119">remove</span><span class="sxs-lookup"><span data-stu-id="f8951-119">remove</span></span>|<span data-ttu-id="f8951-120">1/3</span><span class="sxs-lookup"><span data-stu-id="f8951-120">3</span></span>|<span data-ttu-id="f8951-121">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="f8951-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="f8951-122">使う</span><span class="sxs-lookup"><span data-stu-id="f8951-122">allow</span></span>|<span data-ttu-id="f8951-123">2/4</span><span class="sxs-lookup"><span data-stu-id="f8951-123">4</span></span>|<span data-ttu-id="f8951-124">検出された脅威を許可します。</span><span class="sxs-lookup"><span data-stu-id="f8951-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="f8951-125">自分のもの</span><span class="sxs-lookup"><span data-stu-id="f8951-125">userDefined</span></span>|<span data-ttu-id="f8951-126">5</span><span class="sxs-lookup"><span data-stu-id="f8951-126">5</span></span>|<span data-ttu-id="f8951-127">検出された脅威に対して実行するアクションをユーザーが決定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f8951-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="f8951-128">拒否</span><span class="sxs-lookup"><span data-stu-id="f8951-128">block</span></span>|<span data-ttu-id="f8951-129">シックス</span><span class="sxs-lookup"><span data-stu-id="f8951-129">6</span></span>|<span data-ttu-id="f8951-130">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="f8951-130">Block the detected threat.</span></span>|



