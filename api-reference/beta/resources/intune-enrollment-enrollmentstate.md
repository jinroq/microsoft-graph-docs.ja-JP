---
title: enrollmentState 列挙型
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71f41d459e3fdb50fd853c62a855b4591a8ca8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419108"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="d699f-103">enrollmentState 列挙型</span><span class="sxs-lookup"><span data-stu-id="d699f-103">enrollmentState enum type</span></span>

> <span data-ttu-id="d699f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d699f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d699f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d699f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d699f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d699f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d699f-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d699f-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="d699f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d699f-108">Members</span></span>
|<span data-ttu-id="d699f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d699f-109">Member</span></span>|<span data-ttu-id="d699f-110">値</span><span class="sxs-lookup"><span data-stu-id="d699f-110">Value</span></span>|<span data-ttu-id="d699f-111">説明</span><span class="sxs-lookup"><span data-stu-id="d699f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d699f-112">不明</span><span class="sxs-lookup"><span data-stu-id="d699f-112">unknown</span></span>|<span data-ttu-id="d699f-113">0</span><span class="sxs-lookup"><span data-stu-id="d699f-113">0</span></span>|<span data-ttu-id="d699f-114">デバイス登録の状態は不明です。</span><span class="sxs-lookup"><span data-stu-id="d699f-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="d699f-115">登録</span><span class="sxs-lookup"><span data-stu-id="d699f-115">enrolled</span></span>|<span data-ttu-id="d699f-116">1</span><span class="sxs-lookup"><span data-stu-id="d699f-116">1</span></span>|<span data-ttu-id="d699f-117">デバイスを登録します。</span><span class="sxs-lookup"><span data-stu-id="d699f-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="d699f-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="d699f-118">pendingReset</span></span>|<span data-ttu-id="d699f-119">2</span><span class="sxs-lookup"><span data-stu-id="d699f-119">2</span></span>|<span data-ttu-id="d699f-120">登録され、登録プロファイルを使用して登録されているが、登録されているプロファイルが割り当てられているプロファイルとは異なる。</span><span class="sxs-lookup"><span data-stu-id="d699f-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="d699f-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="d699f-121">failed</span></span>|<span data-ttu-id="d699f-122">3</span><span class="sxs-lookup"><span data-stu-id="d699f-122">3</span></span>|<span data-ttu-id="d699f-123">登録していない登録に失敗したレコードがあるとします。</span><span class="sxs-lookup"><span data-stu-id="d699f-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="d699f-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="d699f-124">notContacted</span></span>|<span data-ttu-id="d699f-125">4</span><span class="sxs-lookup"><span data-stu-id="d699f-125">4</span></span>|<span data-ttu-id="d699f-126">デバイスをインポートしていますが、登録していません。</span><span class="sxs-lookup"><span data-stu-id="d699f-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="d699f-127">ブロック</span><span class="sxs-lookup"><span data-stu-id="d699f-127">blocked</span></span>|<span data-ttu-id="d699f-128">5</span><span class="sxs-lookup"><span data-stu-id="d699f-128">5</span></span>|<span data-ttu-id="d699f-129">デバイスが、userless として登録されて、アプリケーションのインストールに失敗したため、ユーザー登録への移動がブロックされます。</span><span class="sxs-lookup"><span data-stu-id="d699f-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




