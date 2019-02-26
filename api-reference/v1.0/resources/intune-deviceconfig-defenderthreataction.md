---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d3d48415e55ad246f75ca9b32bd169ee102fc67
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252316"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="5be42-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="5be42-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="5be42-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5be42-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5be42-105">検出されたマルウェアの脅威を処理する Defender の既定のアクション。</span><span class="sxs-lookup"><span data-stu-id="5be42-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="5be42-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="5be42-106">Members</span></span>
|<span data-ttu-id="5be42-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5be42-107">Member</span></span>|<span data-ttu-id="5be42-108">値</span><span class="sxs-lookup"><span data-stu-id="5be42-108">Value</span></span>|<span data-ttu-id="5be42-109">説明</span><span class="sxs-lookup"><span data-stu-id="5be42-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5be42-110">devicedefault</span><span class="sxs-lookup"><span data-stu-id="5be42-110">deviceDefault</span></span>|<span data-ttu-id="5be42-111">.0</span><span class="sxs-lookup"><span data-stu-id="5be42-111">0</span></span>|<span data-ttu-id="5be42-112">更新定義に基づいてアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="5be42-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="5be42-113">クリーン</span><span class="sxs-lookup"><span data-stu-id="5be42-113">clean</span></span>|<span data-ttu-id="5be42-114">1-d</span><span class="sxs-lookup"><span data-stu-id="5be42-114">1</span></span>|<span data-ttu-id="5be42-115">検出された脅威を除去します。</span><span class="sxs-lookup"><span data-stu-id="5be42-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="5be42-116">済み</span><span class="sxs-lookup"><span data-stu-id="5be42-116">quarantine</span></span>|<span data-ttu-id="5be42-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5be42-117">2</span></span>|<span data-ttu-id="5be42-118">検出された脅威を検疫します。</span><span class="sxs-lookup"><span data-stu-id="5be42-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="5be42-119">remove</span><span class="sxs-lookup"><span data-stu-id="5be42-119">remove</span></span>|<span data-ttu-id="5be42-120">1/3</span><span class="sxs-lookup"><span data-stu-id="5be42-120">3</span></span>|<span data-ttu-id="5be42-121">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="5be42-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="5be42-122">使う</span><span class="sxs-lookup"><span data-stu-id="5be42-122">allow</span></span>|<span data-ttu-id="5be42-123">2/4</span><span class="sxs-lookup"><span data-stu-id="5be42-123">4</span></span>|<span data-ttu-id="5be42-124">検出された脅威を許可します。</span><span class="sxs-lookup"><span data-stu-id="5be42-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="5be42-125">自分のもの</span><span class="sxs-lookup"><span data-stu-id="5be42-125">userDefined</span></span>|<span data-ttu-id="5be42-126">5</span><span class="sxs-lookup"><span data-stu-id="5be42-126">5</span></span>|<span data-ttu-id="5be42-127">検出された脅威に対して実行するアクションをユーザーが決定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="5be42-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="5be42-128">拒否</span><span class="sxs-lookup"><span data-stu-id="5be42-128">block</span></span>|<span data-ttu-id="5be42-129">シックス</span><span class="sxs-lookup"><span data-stu-id="5be42-129">6</span></span>|<span data-ttu-id="5be42-130">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="5be42-130">Block the detected threat.</span></span>|



