---
title: defenderThreatAction 列挙型
description: Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d092d5a23fc006a9accdf9062a27cd79f323d208
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400271"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="04566-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="04566-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="04566-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04566-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04566-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04566-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04566-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04566-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04566-107">Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。</span><span class="sxs-lookup"><span data-stu-id="04566-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="04566-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="04566-108">Members</span></span>
|<span data-ttu-id="04566-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="04566-109">Member</span></span>|<span data-ttu-id="04566-110">値</span><span class="sxs-lookup"><span data-stu-id="04566-110">Value</span></span>|<span data-ttu-id="04566-111">説明</span><span class="sxs-lookup"><span data-stu-id="04566-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04566-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="04566-112">deviceDefault</span></span>|<span data-ttu-id="04566-113">0</span><span class="sxs-lookup"><span data-stu-id="04566-113">0</span></span>|<span data-ttu-id="04566-114">更新プログラム定義に基づいたアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="04566-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="04566-115">クリーン</span><span class="sxs-lookup"><span data-stu-id="04566-115">clean</span></span>|<span data-ttu-id="04566-116">1</span><span class="sxs-lookup"><span data-stu-id="04566-116">1</span></span>|<span data-ttu-id="04566-117">検出された脅威をクリーニングします。</span><span class="sxs-lookup"><span data-stu-id="04566-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="04566-118">検査</span><span class="sxs-lookup"><span data-stu-id="04566-118">quarantine</span></span>|<span data-ttu-id="04566-119">2</span><span class="sxs-lookup"><span data-stu-id="04566-119">2</span></span>|<span data-ttu-id="04566-120">検出された脅威を隔離します。</span><span class="sxs-lookup"><span data-stu-id="04566-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="04566-121">remove</span><span class="sxs-lookup"><span data-stu-id="04566-121">remove</span></span>|<span data-ttu-id="04566-122">3</span><span class="sxs-lookup"><span data-stu-id="04566-122">3</span></span>|<span data-ttu-id="04566-123">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="04566-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="04566-124">許可します。</span><span class="sxs-lookup"><span data-stu-id="04566-124">allow</span></span>|<span data-ttu-id="04566-125">4</span><span class="sxs-lookup"><span data-stu-id="04566-125">4</span></span>|<span data-ttu-id="04566-126">脅威の検出を許可します。</span><span class="sxs-lookup"><span data-stu-id="04566-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="04566-127">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="04566-127">userDefined</span></span>|<span data-ttu-id="04566-128">5</span><span class="sxs-lookup"><span data-stu-id="04566-128">5</span></span>|<span data-ttu-id="04566-129">検出された脅威に対して実行するアクションを決定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="04566-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="04566-130">ブロック</span><span class="sxs-lookup"><span data-stu-id="04566-130">block</span></span>|<span data-ttu-id="04566-131">6</span><span class="sxs-lookup"><span data-stu-id="04566-131">6</span></span>|<span data-ttu-id="04566-132">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="04566-132">Block the detected threat.</span></span>|




