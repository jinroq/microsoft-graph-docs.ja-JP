---
title: defenderThreatAction 列挙型
description: Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。
ms.openlocfilehash: a5eb108a3ab26596eec9abe838e3bbfe853d96d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023095"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="22117-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="22117-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="22117-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="22117-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22117-105">Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。</span><span class="sxs-lookup"><span data-stu-id="22117-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="22117-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="22117-106">Members</span></span>
|<span data-ttu-id="22117-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="22117-107">Member</span></span>|<span data-ttu-id="22117-108">値</span><span class="sxs-lookup"><span data-stu-id="22117-108">Value</span></span>|<span data-ttu-id="22117-109">説明</span><span class="sxs-lookup"><span data-stu-id="22117-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22117-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="22117-110">deviceDefault</span></span>|<span data-ttu-id="22117-111">0</span><span class="sxs-lookup"><span data-stu-id="22117-111">0</span></span>|<span data-ttu-id="22117-112">更新プログラム定義に基づいたアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="22117-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="22117-113">クリーン</span><span class="sxs-lookup"><span data-stu-id="22117-113">clean</span></span>|<span data-ttu-id="22117-114">1</span><span class="sxs-lookup"><span data-stu-id="22117-114">1</span></span>|<span data-ttu-id="22117-115">検出された脅威をクリーニングします。</span><span class="sxs-lookup"><span data-stu-id="22117-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="22117-116">検査</span><span class="sxs-lookup"><span data-stu-id="22117-116">quarantine</span></span>|<span data-ttu-id="22117-117">2</span><span class="sxs-lookup"><span data-stu-id="22117-117">2</span></span>|<span data-ttu-id="22117-118">検出された脅威を隔離します。</span><span class="sxs-lookup"><span data-stu-id="22117-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="22117-119">remove</span><span class="sxs-lookup"><span data-stu-id="22117-119">remove</span></span>|<span data-ttu-id="22117-120">3</span><span class="sxs-lookup"><span data-stu-id="22117-120">3</span></span>|<span data-ttu-id="22117-121">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="22117-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="22117-122">許可します。</span><span class="sxs-lookup"><span data-stu-id="22117-122">allow</span></span>|<span data-ttu-id="22117-123">4</span><span class="sxs-lookup"><span data-stu-id="22117-123">4</span></span>|<span data-ttu-id="22117-124">脅威の検出を許可します。</span><span class="sxs-lookup"><span data-stu-id="22117-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="22117-125">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="22117-125">userDefined</span></span>|<span data-ttu-id="22117-126">5</span><span class="sxs-lookup"><span data-stu-id="22117-126">5</span></span>|<span data-ttu-id="22117-127">検出された脅威に対して実行するアクションを決定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="22117-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="22117-128">ブロック</span><span class="sxs-lookup"><span data-stu-id="22117-128">block</span></span>|<span data-ttu-id="22117-129">6</span><span class="sxs-lookup"><span data-stu-id="22117-129">6</span></span>|<span data-ttu-id="22117-130">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="22117-130">Block the detected threat.</span></span>|



