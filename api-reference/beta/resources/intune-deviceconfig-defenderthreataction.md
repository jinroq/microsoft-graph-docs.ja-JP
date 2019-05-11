---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1376927bc76903e10619e7c71fa53ce26d17075
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947296"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="85757-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="85757-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="85757-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85757-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85757-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="85757-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85757-106">検出されたマルウェアの脅威を処理する Defender の既定のアクション。</span><span class="sxs-lookup"><span data-stu-id="85757-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="85757-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="85757-107">Members</span></span>
|<span data-ttu-id="85757-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="85757-108">Member</span></span>|<span data-ttu-id="85757-109">値</span><span class="sxs-lookup"><span data-stu-id="85757-109">Value</span></span>|<span data-ttu-id="85757-110">説明</span><span class="sxs-lookup"><span data-stu-id="85757-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85757-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="85757-111">deviceDefault</span></span>|<span data-ttu-id="85757-112">.0</span><span class="sxs-lookup"><span data-stu-id="85757-112">0</span></span>|<span data-ttu-id="85757-113">更新定義に基づいてアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="85757-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="85757-114">汚れ</span><span class="sxs-lookup"><span data-stu-id="85757-114">clean</span></span>|<span data-ttu-id="85757-115">1-d</span><span class="sxs-lookup"><span data-stu-id="85757-115">1</span></span>|<span data-ttu-id="85757-116">検出された脅威を除去します。</span><span class="sxs-lookup"><span data-stu-id="85757-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="85757-117">済み</span><span class="sxs-lookup"><span data-stu-id="85757-117">quarantine</span></span>|<span data-ttu-id="85757-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="85757-118">2</span></span>|<span data-ttu-id="85757-119">検出された脅威を検疫します。</span><span class="sxs-lookup"><span data-stu-id="85757-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="85757-120">remove</span><span class="sxs-lookup"><span data-stu-id="85757-120">remove</span></span>|<span data-ttu-id="85757-121">1/3</span><span class="sxs-lookup"><span data-stu-id="85757-121">3</span></span>|<span data-ttu-id="85757-122">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="85757-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="85757-123">使う</span><span class="sxs-lookup"><span data-stu-id="85757-123">allow</span></span>|<span data-ttu-id="85757-124">2/4</span><span class="sxs-lookup"><span data-stu-id="85757-124">4</span></span>|<span data-ttu-id="85757-125">検出された脅威を許可します。</span><span class="sxs-lookup"><span data-stu-id="85757-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="85757-126">自分のもの</span><span class="sxs-lookup"><span data-stu-id="85757-126">userDefined</span></span>|<span data-ttu-id="85757-127">5</span><span class="sxs-lookup"><span data-stu-id="85757-127">5</span></span>|<span data-ttu-id="85757-128">検出された脅威に対して実行するアクションをユーザーが決定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="85757-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="85757-129">拒否</span><span class="sxs-lookup"><span data-stu-id="85757-129">block</span></span>|<span data-ttu-id="85757-130">シックス</span><span class="sxs-lookup"><span data-stu-id="85757-130">6</span></span>|<span data-ttu-id="85757-131">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="85757-131">Block the detected threat.</span></span>|




