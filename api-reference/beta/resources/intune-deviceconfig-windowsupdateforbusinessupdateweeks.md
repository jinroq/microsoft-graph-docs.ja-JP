---
title: windowsUpdateForBusinessUpdateWeeks 列挙型
description: 月の週に更新プログラムのインストールをスケジュールします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a6f35efcc7ceb585a6c717459d810c274d2bc69f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957317"
---
# <a name="windowsupdateforbusinessupdateweeks-enum-type"></a><span data-ttu-id="dc5ab-103">windowsUpdateForBusinessUpdateWeeks 列挙型</span><span class="sxs-lookup"><span data-stu-id="dc5ab-103">windowsUpdateForBusinessUpdateWeeks enum type</span></span>

> <span data-ttu-id="dc5ab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc5ab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc5ab-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc5ab-107">月の週に更新プログラムのインストールをスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-107">Scheduled the update installation on the weeks of the month</span></span>
## <a name="members"></a><span data-ttu-id="dc5ab-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc5ab-108">Members</span></span>
|<span data-ttu-id="dc5ab-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="dc5ab-109">Member</span></span>|<span data-ttu-id="dc5ab-110">値</span><span class="sxs-lookup"><span data-stu-id="dc5ab-110">Value</span></span>|<span data-ttu-id="dc5ab-111">説明</span><span class="sxs-lookup"><span data-stu-id="dc5ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc5ab-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="dc5ab-112">userDefined</span></span>|<span data-ttu-id="dc5ab-113">0</span><span class="sxs-lookup"><span data-stu-id="dc5ab-113">0</span></span>|<span data-ttu-id="dc5ab-114">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-114">Allow the user to set.</span></span>|
|<span data-ttu-id="dc5ab-115">firstWeek</span><span class="sxs-lookup"><span data-stu-id="dc5ab-115">firstWeek</span></span>|<span data-ttu-id="dc5ab-116">1</span><span class="sxs-lookup"><span data-stu-id="dc5ab-116">1</span></span>|<span data-ttu-id="dc5ab-117">月の最初の週に更新プログラムのインストールをスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-117">Scheduled the update installation on the first week of the month</span></span>|
|<span data-ttu-id="dc5ab-118">secondWeek</span><span class="sxs-lookup"><span data-stu-id="dc5ab-118">secondWeek</span></span>|<span data-ttu-id="dc5ab-119">2</span><span class="sxs-lookup"><span data-stu-id="dc5ab-119">2</span></span>|<span data-ttu-id="dc5ab-120">月の第 2 週に更新プログラムのインストールをスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-120">Scheduled the update installation on the second week of the month</span></span>|
|<span data-ttu-id="dc5ab-121">thirdWeek</span><span class="sxs-lookup"><span data-stu-id="dc5ab-121">thirdWeek</span></span>|<span data-ttu-id="dc5ab-122">4</span><span class="sxs-lookup"><span data-stu-id="dc5ab-122">4</span></span>|<span data-ttu-id="dc5ab-123">月の第 3 週に更新プログラムのインストールをスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-123">Scheduled the update installation on the third week of the month</span></span>|
|<span data-ttu-id="dc5ab-124">fourthWeek</span><span class="sxs-lookup"><span data-stu-id="dc5ab-124">fourthWeek</span></span>|<span data-ttu-id="dc5ab-125">8</span><span class="sxs-lookup"><span data-stu-id="dc5ab-125">8</span></span>|<span data-ttu-id="dc5ab-126">月の第 4 週に更新プログラムのインストールをスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-126">Scheduled the update installation on the fourth week of the month</span></span>|
|<span data-ttu-id="dc5ab-127">everyWeek</span><span class="sxs-lookup"><span data-stu-id="dc5ab-127">everyWeek</span></span>|<span data-ttu-id="dc5ab-128">15</span><span class="sxs-lookup"><span data-stu-id="dc5ab-128">15</span></span>|<span data-ttu-id="dc5ab-129">月の毎週の更新プログラムのインストールをスケジュールします。</span><span class="sxs-lookup"><span data-stu-id="dc5ab-129">Scheduled the update installation on every week of the month</span></span>|





