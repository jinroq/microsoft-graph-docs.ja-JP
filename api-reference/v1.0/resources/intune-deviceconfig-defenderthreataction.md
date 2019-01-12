---
title: defenderThreatAction 列挙型
description: Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 51aa26483ac6b79d48567f7e5950733def31f01e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976647"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="313cb-103">defenderThreatAction 列挙型</span><span class="sxs-lookup"><span data-stu-id="313cb-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="313cb-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="313cb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="313cb-105">Defender の既定のアクション実行するには、マルウェアの脅威が検出されました。</span><span class="sxs-lookup"><span data-stu-id="313cb-105">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="313cb-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="313cb-106">Members</span></span>
|<span data-ttu-id="313cb-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="313cb-107">Member</span></span>|<span data-ttu-id="313cb-108">値</span><span class="sxs-lookup"><span data-stu-id="313cb-108">Value</span></span>|<span data-ttu-id="313cb-109">説明</span><span class="sxs-lookup"><span data-stu-id="313cb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="313cb-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="313cb-110">deviceDefault</span></span>|<span data-ttu-id="313cb-111">0</span><span class="sxs-lookup"><span data-stu-id="313cb-111">0</span></span>|<span data-ttu-id="313cb-112">更新プログラム定義に基づいたアクションを適用します。</span><span class="sxs-lookup"><span data-stu-id="313cb-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="313cb-113">クリーン</span><span class="sxs-lookup"><span data-stu-id="313cb-113">clean</span></span>|<span data-ttu-id="313cb-114">1</span><span class="sxs-lookup"><span data-stu-id="313cb-114">1</span></span>|<span data-ttu-id="313cb-115">検出された脅威をクリーニングします。</span><span class="sxs-lookup"><span data-stu-id="313cb-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="313cb-116">検査</span><span class="sxs-lookup"><span data-stu-id="313cb-116">quarantine</span></span>|<span data-ttu-id="313cb-117">2</span><span class="sxs-lookup"><span data-stu-id="313cb-117">2</span></span>|<span data-ttu-id="313cb-118">検出された脅威を隔離します。</span><span class="sxs-lookup"><span data-stu-id="313cb-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="313cb-119">remove</span><span class="sxs-lookup"><span data-stu-id="313cb-119">remove</span></span>|<span data-ttu-id="313cb-120">3</span><span class="sxs-lookup"><span data-stu-id="313cb-120">3</span></span>|<span data-ttu-id="313cb-121">検出された脅威を削除します。</span><span class="sxs-lookup"><span data-stu-id="313cb-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="313cb-122">許可します。</span><span class="sxs-lookup"><span data-stu-id="313cb-122">allow</span></span>|<span data-ttu-id="313cb-123">4</span><span class="sxs-lookup"><span data-stu-id="313cb-123">4</span></span>|<span data-ttu-id="313cb-124">脅威の検出を許可します。</span><span class="sxs-lookup"><span data-stu-id="313cb-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="313cb-125">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="313cb-125">userDefined</span></span>|<span data-ttu-id="313cb-126">5</span><span class="sxs-lookup"><span data-stu-id="313cb-126">5</span></span>|<span data-ttu-id="313cb-127">検出された脅威に対して実行するアクションを決定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="313cb-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="313cb-128">ブロック</span><span class="sxs-lookup"><span data-stu-id="313cb-128">block</span></span>|<span data-ttu-id="313cb-129">6</span><span class="sxs-lookup"><span data-stu-id="313cb-129">6</span></span>|<span data-ttu-id="313cb-130">検出された脅威をブロックします。</span><span class="sxs-lookup"><span data-stu-id="313cb-130">Block the detected threat.</span></span>|



