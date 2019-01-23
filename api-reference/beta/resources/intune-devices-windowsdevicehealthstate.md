---
title: windowsDeviceHealthState 列挙型
description: コンピューター エンドポイントの保護の状態
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416350"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="eb9af-103">windowsDeviceHealthState 列挙型</span><span class="sxs-lookup"><span data-stu-id="eb9af-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="eb9af-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eb9af-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eb9af-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb9af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb9af-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb9af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb9af-107">コンピューター エンドポイントの保護の状態</span><span class="sxs-lookup"><span data-stu-id="eb9af-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="eb9af-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="eb9af-108">Members</span></span>
|<span data-ttu-id="eb9af-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="eb9af-109">Member</span></span>|<span data-ttu-id="eb9af-110">値</span><span class="sxs-lookup"><span data-stu-id="eb9af-110">Value</span></span>|<span data-ttu-id="eb9af-111">説明</span><span class="sxs-lookup"><span data-stu-id="eb9af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb9af-112">クリーン</span><span class="sxs-lookup"><span data-stu-id="eb9af-112">clean</span></span>|<span data-ttu-id="eb9af-113">0</span><span class="sxs-lookup"><span data-stu-id="eb9af-113">0</span></span>|<span data-ttu-id="eb9af-114">コンピューターがクリーンであり、操作する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="eb9af-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="eb9af-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="eb9af-115">fullScanPending</span></span>|<span data-ttu-id="eb9af-116">1</span><span class="sxs-lookup"><span data-stu-id="eb9af-116">1</span></span>|<span data-ttu-id="eb9af-117">コンピューターで保留中の状態の完全なスキャンは、</span><span class="sxs-lookup"><span data-stu-id="eb9af-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="eb9af-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="eb9af-118">rebootPending</span></span>|<span data-ttu-id="eb9af-119">2</span><span class="sxs-lookup"><span data-stu-id="eb9af-119">2</span></span>|<span data-ttu-id="eb9af-120">コンピューターで保留中の再起動の状態には</span><span class="sxs-lookup"><span data-stu-id="eb9af-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="eb9af-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="eb9af-121">manualStepsPending</span></span>|<span data-ttu-id="eb9af-122">4</span><span class="sxs-lookup"><span data-stu-id="eb9af-122">4</span></span>|<span data-ttu-id="eb9af-123">コンピューターで保留中の手動の手順の状態は、</span><span class="sxs-lookup"><span data-stu-id="eb9af-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="eb9af-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="eb9af-124">offlineScanPending</span></span>|<span data-ttu-id="eb9af-125">8</span><span class="sxs-lookup"><span data-stu-id="eb9af-125">8</span></span>|<span data-ttu-id="eb9af-126">オフライン スキャンの状態を保留中のコンピューターが、します。</span><span class="sxs-lookup"><span data-stu-id="eb9af-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="eb9af-127">critical</span><span class="sxs-lookup"><span data-stu-id="eb9af-127">critical</span></span>|<span data-ttu-id="eb9af-128">16</span><span class="sxs-lookup"><span data-stu-id="eb9af-128">16</span></span>|<span data-ttu-id="eb9af-129">コンピューターが、重大なエラー状態</span><span class="sxs-lookup"><span data-stu-id="eb9af-129">Computer is in critical failure state</span></span>|




