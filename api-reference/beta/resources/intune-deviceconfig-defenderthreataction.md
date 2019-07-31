---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 368d58c125511f235a82d50e54193f0dacc96757
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970851"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="3fb7f-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="3fb7f-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="3fb7f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fb7f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fb7f-106">検出されたマルウェアの脅威を処理する Defender の既定のアクション。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="3fb7f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fb7f-107">Members</span></span>
|<span data-ttu-id="3fb7f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fb7f-108">Member</span></span>|<span data-ttu-id="3fb7f-109">値</span><span class="sxs-lookup"><span data-stu-id="3fb7f-109">Value</span></span>|<span data-ttu-id="3fb7f-110">説明</span><span class="sxs-lookup"><span data-stu-id="3fb7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fb7f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3fb7f-111">deviceDefault</span></span>|<span data-ttu-id="3fb7f-112">.0</span><span class="sxs-lookup"><span data-stu-id="3fb7f-112">0</span></span>|<span data-ttu-id="3fb7f-113">更新定義に基づいてアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="3fb7f-114">汚れ</span><span class="sxs-lookup"><span data-stu-id="3fb7f-114">clean</span></span>|<span data-ttu-id="3fb7f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3fb7f-115">1</span></span>|<span data-ttu-id="3fb7f-116">検出された脅威を除去します。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="3fb7f-117">済み</span><span class="sxs-lookup"><span data-stu-id="3fb7f-117">quarantine</span></span>|<span data-ttu-id="3fb7f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3fb7f-118">2</span></span>|<span data-ttu-id="3fb7f-119">検出された脅威を検疫します。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="3fb7f-120">remove</span><span class="sxs-lookup"><span data-stu-id="3fb7f-120">remove</span></span>|<span data-ttu-id="3fb7f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3fb7f-121">3</span></span>|<span data-ttu-id="3fb7f-122">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="3fb7f-123">使う</span><span class="sxs-lookup"><span data-stu-id="3fb7f-123">allow</span></span>|<span data-ttu-id="3fb7f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="3fb7f-124">4</span></span>|<span data-ttu-id="3fb7f-125">検出された脅威を許可します。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="3fb7f-126">自分のもの</span><span class="sxs-lookup"><span data-stu-id="3fb7f-126">userDefined</span></span>|<span data-ttu-id="3fb7f-127">5</span><span class="sxs-lookup"><span data-stu-id="3fb7f-127">5</span></span>|<span data-ttu-id="3fb7f-128">検出された脅威に対して実行するアクションをユーザーが決定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="3fb7f-129">拒否</span><span class="sxs-lookup"><span data-stu-id="3fb7f-129">block</span></span>|<span data-ttu-id="3fb7f-130">シックス</span><span class="sxs-lookup"><span data-stu-id="3fb7f-130">6</span></span>|<span data-ttu-id="3fb7f-131">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="3fb7f-131">Block the detected threat.</span></span>|





