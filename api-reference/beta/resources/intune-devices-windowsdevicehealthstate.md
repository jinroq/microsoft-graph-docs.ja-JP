---
title: windowsDeviceHealthState 列挙型
description: コンピューター エンドポイントの保護の状態
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923944"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="4f5be-103">windowsDeviceHealthState 列挙型</span><span class="sxs-lookup"><span data-stu-id="4f5be-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="4f5be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4f5be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f5be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f5be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f5be-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f5be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f5be-107">コンピューター エンドポイントの保護の状態</span><span class="sxs-lookup"><span data-stu-id="4f5be-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="4f5be-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f5be-108">Members</span></span>
|<span data-ttu-id="4f5be-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4f5be-109">Member</span></span>|<span data-ttu-id="4f5be-110">値</span><span class="sxs-lookup"><span data-stu-id="4f5be-110">Value</span></span>|<span data-ttu-id="4f5be-111">説明</span><span class="sxs-lookup"><span data-stu-id="4f5be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f5be-112">クリーン</span><span class="sxs-lookup"><span data-stu-id="4f5be-112">clean</span></span>|<span data-ttu-id="4f5be-113">0</span><span class="sxs-lookup"><span data-stu-id="4f5be-113">0</span></span>|<span data-ttu-id="4f5be-114">コンピューターがクリーンであり、操作する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="4f5be-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="4f5be-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="4f5be-115">fullScanPending</span></span>|<span data-ttu-id="4f5be-116">1</span><span class="sxs-lookup"><span data-stu-id="4f5be-116">1</span></span>|<span data-ttu-id="4f5be-117">コンピューターで保留中の状態の完全なスキャンは、</span><span class="sxs-lookup"><span data-stu-id="4f5be-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="4f5be-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="4f5be-118">rebootPending</span></span>|<span data-ttu-id="4f5be-119">2</span><span class="sxs-lookup"><span data-stu-id="4f5be-119">2</span></span>|<span data-ttu-id="4f5be-120">コンピューターで保留中の再起動の状態には</span><span class="sxs-lookup"><span data-stu-id="4f5be-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="4f5be-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="4f5be-121">manualStepsPending</span></span>|<span data-ttu-id="4f5be-122">4</span><span class="sxs-lookup"><span data-stu-id="4f5be-122">4</span></span>|<span data-ttu-id="4f5be-123">コンピューターで保留中の手動の手順の状態は、</span><span class="sxs-lookup"><span data-stu-id="4f5be-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="4f5be-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="4f5be-124">offlineScanPending</span></span>|<span data-ttu-id="4f5be-125">8</span><span class="sxs-lookup"><span data-stu-id="4f5be-125">8</span></span>|<span data-ttu-id="4f5be-126">オフライン スキャンの状態を保留中のコンピューターが、します。</span><span class="sxs-lookup"><span data-stu-id="4f5be-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="4f5be-127">critical</span><span class="sxs-lookup"><span data-stu-id="4f5be-127">critical</span></span>|<span data-ttu-id="4f5be-128">16</span><span class="sxs-lookup"><span data-stu-id="4f5be-128">16</span></span>|<span data-ttu-id="4f5be-129">コンピューターが、重大なエラー状態</span><span class="sxs-lookup"><span data-stu-id="4f5be-129">Computer is in critical failure state</span></span>|





