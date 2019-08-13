---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 57b5ecf73548bf67bcb1fbfb75ed0730cb308424
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333416"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="47244-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="47244-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="47244-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47244-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47244-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47244-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47244-106">検出されたマルウェアの脅威を処理する Defender の既定のアクション。</span><span class="sxs-lookup"><span data-stu-id="47244-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="47244-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="47244-107">Members</span></span>
|<span data-ttu-id="47244-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="47244-108">Member</span></span>|<span data-ttu-id="47244-109">値</span><span class="sxs-lookup"><span data-stu-id="47244-109">Value</span></span>|<span data-ttu-id="47244-110">説明</span><span class="sxs-lookup"><span data-stu-id="47244-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47244-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="47244-111">deviceDefault</span></span>|<span data-ttu-id="47244-112">.0</span><span class="sxs-lookup"><span data-stu-id="47244-112">0</span></span>|<span data-ttu-id="47244-113">更新定義に基づいてアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="47244-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="47244-114">汚れ</span><span class="sxs-lookup"><span data-stu-id="47244-114">clean</span></span>|<span data-ttu-id="47244-115">1-d</span><span class="sxs-lookup"><span data-stu-id="47244-115">1</span></span>|<span data-ttu-id="47244-116">検出された脅威を除去します。</span><span class="sxs-lookup"><span data-stu-id="47244-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="47244-117">済み</span><span class="sxs-lookup"><span data-stu-id="47244-117">quarantine</span></span>|<span data-ttu-id="47244-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="47244-118">2</span></span>|<span data-ttu-id="47244-119">検出された脅威を検疫します。</span><span class="sxs-lookup"><span data-stu-id="47244-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="47244-120">remove</span><span class="sxs-lookup"><span data-stu-id="47244-120">remove</span></span>|<span data-ttu-id="47244-121">1/3</span><span class="sxs-lookup"><span data-stu-id="47244-121">3</span></span>|<span data-ttu-id="47244-122">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="47244-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="47244-123">使う</span><span class="sxs-lookup"><span data-stu-id="47244-123">allow</span></span>|<span data-ttu-id="47244-124">2/4</span><span class="sxs-lookup"><span data-stu-id="47244-124">4</span></span>|<span data-ttu-id="47244-125">検出された脅威を許可します。</span><span class="sxs-lookup"><span data-stu-id="47244-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="47244-126">自分のもの</span><span class="sxs-lookup"><span data-stu-id="47244-126">userDefined</span></span>|<span data-ttu-id="47244-127">5</span><span class="sxs-lookup"><span data-stu-id="47244-127">5</span></span>|<span data-ttu-id="47244-128">検出された脅威に対して実行するアクションをユーザーが決定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="47244-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="47244-129">拒否</span><span class="sxs-lookup"><span data-stu-id="47244-129">block</span></span>|<span data-ttu-id="47244-130">シックス</span><span class="sxs-lookup"><span data-stu-id="47244-130">6</span></span>|<span data-ttu-id="47244-131">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="47244-131">Block the detected threat.</span></span>|



