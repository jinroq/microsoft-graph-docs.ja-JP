---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
author: tfitzmac
ms.openlocfilehash: 19498f587759df56ae671b119b59abe7e7acd62c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314932"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="ec5e8-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="ec5e8-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="ec5e8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec5e8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec5e8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec5e8-107">サンプル提出用のユーザーにメッセージを表示可能な値です。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-107">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="ec5e8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec5e8-108">Members</span></span>
|<span data-ttu-id="ec5e8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec5e8-109">Member</span></span>|<span data-ttu-id="ec5e8-110">値</span><span class="sxs-lookup"><span data-stu-id="ec5e8-110">Value</span></span>|<span data-ttu-id="ec5e8-111">説明</span><span class="sxs-lookup"><span data-stu-id="ec5e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec5e8-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="ec5e8-112">userDefined</span></span>|<span data-ttu-id="ec5e8-113">0</span><span class="sxs-lookup"><span data-stu-id="ec5e8-113">0</span></span>|<span data-ttu-id="ec5e8-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ec5e8-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="ec5e8-115">alwaysPrompt</span></span>|<span data-ttu-id="ec5e8-116">1</span><span class="sxs-lookup"><span data-stu-id="ec5e8-116">1</span></span>|<span data-ttu-id="ec5e8-117">常にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-117">Always prompt.</span></span>|
|<span data-ttu-id="ec5e8-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="ec5e8-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="ec5e8-119">2</span><span class="sxs-lookup"><span data-stu-id="ec5e8-119">2</span></span>|<span data-ttu-id="ec5e8-120">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="ec5e8-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="ec5e8-121">neverSendData</span></span>|<span data-ttu-id="ec5e8-122">3</span><span class="sxs-lookup"><span data-stu-id="ec5e8-122">3</span></span>|<span data-ttu-id="ec5e8-123">データを送信しないでください。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-123">Never send data.</span></span>|
|<span data-ttu-id="ec5e8-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="ec5e8-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="ec5e8-125">4</span><span class="sxs-lookup"><span data-stu-id="ec5e8-125">4</span></span>|<span data-ttu-id="ec5e8-126">メッセージを表示せず、すべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="ec5e8-126">Send all data without prompting.</span></span>|





