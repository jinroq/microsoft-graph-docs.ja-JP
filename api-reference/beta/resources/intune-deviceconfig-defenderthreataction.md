---
title: defenderThreatAction 列挙型
description: Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。
localization_priority: Normal
ms.openlocfilehash: 7e448e6fae0ebbb0f14a3b7932e6f306a70588b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837871"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="06434-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="06434-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="06434-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="06434-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06434-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06434-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06434-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="06434-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06434-107">Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。</span><span class="sxs-lookup"><span data-stu-id="06434-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="06434-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="06434-108">Members</span></span>
|<span data-ttu-id="06434-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="06434-109">Member</span></span>|<span data-ttu-id="06434-110">値</span><span class="sxs-lookup"><span data-stu-id="06434-110">Value</span></span>|<span data-ttu-id="06434-111">説明</span><span class="sxs-lookup"><span data-stu-id="06434-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06434-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="06434-112">deviceDefault</span></span>|<span data-ttu-id="06434-113">0</span><span class="sxs-lookup"><span data-stu-id="06434-113">0</span></span>|<span data-ttu-id="06434-114">更新プログラム定義に基づいたアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="06434-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="06434-115">クリーン</span><span class="sxs-lookup"><span data-stu-id="06434-115">clean</span></span>|<span data-ttu-id="06434-116">1</span><span class="sxs-lookup"><span data-stu-id="06434-116">1</span></span>|<span data-ttu-id="06434-117">検出された脅威をクリーニングします。</span><span class="sxs-lookup"><span data-stu-id="06434-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="06434-118">検査</span><span class="sxs-lookup"><span data-stu-id="06434-118">quarantine</span></span>|<span data-ttu-id="06434-119">2</span><span class="sxs-lookup"><span data-stu-id="06434-119">2</span></span>|<span data-ttu-id="06434-120">検出された脅威を隔離します。</span><span class="sxs-lookup"><span data-stu-id="06434-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="06434-121">remove</span><span class="sxs-lookup"><span data-stu-id="06434-121">remove</span></span>|<span data-ttu-id="06434-122">3</span><span class="sxs-lookup"><span data-stu-id="06434-122">3</span></span>|<span data-ttu-id="06434-123">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="06434-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="06434-124">許可します。</span><span class="sxs-lookup"><span data-stu-id="06434-124">allow</span></span>|<span data-ttu-id="06434-125">4</span><span class="sxs-lookup"><span data-stu-id="06434-125">4</span></span>|<span data-ttu-id="06434-126">脅威の検出を許可します。</span><span class="sxs-lookup"><span data-stu-id="06434-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="06434-127">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="06434-127">userDefined</span></span>|<span data-ttu-id="06434-128">5</span><span class="sxs-lookup"><span data-stu-id="06434-128">5</span></span>|<span data-ttu-id="06434-129">検出された脅威に対して実行するアクションを決定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="06434-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="06434-130">ブロック</span><span class="sxs-lookup"><span data-stu-id="06434-130">block</span></span>|<span data-ttu-id="06434-131">6</span><span class="sxs-lookup"><span data-stu-id="06434-131">6</span></span>|<span data-ttu-id="06434-132">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="06434-132">Block the detected threat.</span></span>|





