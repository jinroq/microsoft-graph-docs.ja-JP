---
title: defenderThreatAction 列挙型
description: 検出されたマルウェアの脅威を処理する Defender の既定のアクション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e16ea7734b61213286d15467701fa3512ebb7d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563820"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="d9c36-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="d9c36-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="d9c36-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d9c36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9c36-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d9c36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9c36-106">検出されたマルウェアの脅威を処理する Defender の既定のアクション。</span><span class="sxs-lookup"><span data-stu-id="d9c36-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="d9c36-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9c36-107">Members</span></span>
|<span data-ttu-id="d9c36-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9c36-108">Member</span></span>|<span data-ttu-id="d9c36-109">値</span><span class="sxs-lookup"><span data-stu-id="d9c36-109">Value</span></span>|<span data-ttu-id="d9c36-110">説明</span><span class="sxs-lookup"><span data-stu-id="d9c36-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9c36-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="d9c36-111">deviceDefault</span></span>|<span data-ttu-id="d9c36-112">.0</span><span class="sxs-lookup"><span data-stu-id="d9c36-112">0</span></span>|<span data-ttu-id="d9c36-113">更新定義に基づいてアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="d9c36-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="d9c36-114">汚れ</span><span class="sxs-lookup"><span data-stu-id="d9c36-114">clean</span></span>|<span data-ttu-id="d9c36-115">1 </span><span class="sxs-lookup"><span data-stu-id="d9c36-115">1</span></span>|<span data-ttu-id="d9c36-116">検出された脅威を除去します。</span><span class="sxs-lookup"><span data-stu-id="d9c36-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="d9c36-117">済み</span><span class="sxs-lookup"><span data-stu-id="d9c36-117">quarantine</span></span>|<span data-ttu-id="d9c36-118">2 </span><span class="sxs-lookup"><span data-stu-id="d9c36-118">2</span></span>|<span data-ttu-id="d9c36-119">検出された脅威を検疫します。</span><span class="sxs-lookup"><span data-stu-id="d9c36-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="d9c36-120">remove</span><span class="sxs-lookup"><span data-stu-id="d9c36-120">remove</span></span>|<span data-ttu-id="d9c36-121">3 </span><span class="sxs-lookup"><span data-stu-id="d9c36-121">3</span></span>|<span data-ttu-id="d9c36-122">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="d9c36-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="d9c36-123">使う</span><span class="sxs-lookup"><span data-stu-id="d9c36-123">allow</span></span>|<span data-ttu-id="d9c36-124">4 </span><span class="sxs-lookup"><span data-stu-id="d9c36-124">4</span></span>|<span data-ttu-id="d9c36-125">検出された脅威を許可します。</span><span class="sxs-lookup"><span data-stu-id="d9c36-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="d9c36-126">自分のもの</span><span class="sxs-lookup"><span data-stu-id="d9c36-126">userDefined</span></span>|<span data-ttu-id="d9c36-127">5 </span><span class="sxs-lookup"><span data-stu-id="d9c36-127">5</span></span>|<span data-ttu-id="d9c36-128">検出された脅威に対して実行するアクションをユーザーが決定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d9c36-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="d9c36-129">拒否</span><span class="sxs-lookup"><span data-stu-id="d9c36-129">block</span></span>|<span data-ttu-id="d9c36-130">6 </span><span class="sxs-lookup"><span data-stu-id="d9c36-130">6</span></span>|<span data-ttu-id="d9c36-131">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="d9c36-131">Block the detected threat.</span></span>|





