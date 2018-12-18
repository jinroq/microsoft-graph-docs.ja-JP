---
title: windowsDeviceHealthState 列挙型
description: コンピューター エンドポイントの保護の状態
author: tfitzmac
ms.openlocfilehash: b794f8121132e396459f9198c644084690fe95b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326328"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="71f61-103">windowsDeviceHealthState 列挙型</span><span class="sxs-lookup"><span data-stu-id="71f61-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="71f61-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="71f61-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71f61-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71f61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71f61-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="71f61-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71f61-107">コンピューター エンドポイントの保護の状態</span><span class="sxs-lookup"><span data-stu-id="71f61-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="71f61-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="71f61-108">Members</span></span>
|<span data-ttu-id="71f61-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="71f61-109">Member</span></span>|<span data-ttu-id="71f61-110">値</span><span class="sxs-lookup"><span data-stu-id="71f61-110">Value</span></span>|<span data-ttu-id="71f61-111">説明</span><span class="sxs-lookup"><span data-stu-id="71f61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f61-112">クリーン</span><span class="sxs-lookup"><span data-stu-id="71f61-112">clean</span></span>|<span data-ttu-id="71f61-113">0</span><span class="sxs-lookup"><span data-stu-id="71f61-113">0</span></span>|<span data-ttu-id="71f61-114">コンピューターがクリーンであり、操作する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="71f61-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="71f61-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="71f61-115">fullScanPending</span></span>|<span data-ttu-id="71f61-116">1</span><span class="sxs-lookup"><span data-stu-id="71f61-116">1</span></span>|<span data-ttu-id="71f61-117">コンピューターで保留中の状態の完全なスキャンは、</span><span class="sxs-lookup"><span data-stu-id="71f61-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="71f61-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="71f61-118">rebootPending</span></span>|<span data-ttu-id="71f61-119">2</span><span class="sxs-lookup"><span data-stu-id="71f61-119">2</span></span>|<span data-ttu-id="71f61-120">コンピューターで保留中の再起動の状態には</span><span class="sxs-lookup"><span data-stu-id="71f61-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="71f61-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="71f61-121">manualStepsPending</span></span>|<span data-ttu-id="71f61-122">4</span><span class="sxs-lookup"><span data-stu-id="71f61-122">4</span></span>|<span data-ttu-id="71f61-123">コンピューターで保留中の手動の手順の状態は、</span><span class="sxs-lookup"><span data-stu-id="71f61-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="71f61-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="71f61-124">offlineScanPending</span></span>|<span data-ttu-id="71f61-125">8</span><span class="sxs-lookup"><span data-stu-id="71f61-125">8</span></span>|<span data-ttu-id="71f61-126">オフライン スキャンの状態を保留中のコンピューターが、します。</span><span class="sxs-lookup"><span data-stu-id="71f61-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="71f61-127">critical</span><span class="sxs-lookup"><span data-stu-id="71f61-127">critical</span></span>|<span data-ttu-id="71f61-128">16</span><span class="sxs-lookup"><span data-stu-id="71f61-128">16</span></span>|<span data-ttu-id="71f61-129">コンピューターが、重大なエラー状態</span><span class="sxs-lookup"><span data-stu-id="71f61-129">Computer is in critical failure state</span></span>|





