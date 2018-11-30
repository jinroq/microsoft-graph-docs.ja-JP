---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
ms.openlocfilehash: b70e86cb010395d5c3dfbd3266cc0cb7f6383fbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068241"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="feceb-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="feceb-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="feceb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="feceb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="feceb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="feceb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="feceb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="feceb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="feceb-107">サンプル提出用のユーザーにメッセージを表示可能な値です。</span><span class="sxs-lookup"><span data-stu-id="feceb-107">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="feceb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="feceb-108">Members</span></span>
|<span data-ttu-id="feceb-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="feceb-109">Member</span></span>|<span data-ttu-id="feceb-110">値</span><span class="sxs-lookup"><span data-stu-id="feceb-110">Value</span></span>|<span data-ttu-id="feceb-111">説明</span><span class="sxs-lookup"><span data-stu-id="feceb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feceb-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="feceb-112">userDefined</span></span>|<span data-ttu-id="feceb-113">0</span><span class="sxs-lookup"><span data-stu-id="feceb-113">0</span></span>|<span data-ttu-id="feceb-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="feceb-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="feceb-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="feceb-115">alwaysPrompt</span></span>|<span data-ttu-id="feceb-116">1</span><span class="sxs-lookup"><span data-stu-id="feceb-116">1</span></span>|<span data-ttu-id="feceb-117">常にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="feceb-117">Always prompt.</span></span>|
|<span data-ttu-id="feceb-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="feceb-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="feceb-119">2</span><span class="sxs-lookup"><span data-stu-id="feceb-119">2</span></span>|<span data-ttu-id="feceb-120">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="feceb-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="feceb-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="feceb-121">neverSendData</span></span>|<span data-ttu-id="feceb-122">3</span><span class="sxs-lookup"><span data-stu-id="feceb-122">3</span></span>|<span data-ttu-id="feceb-123">データを送信しないでください。</span><span class="sxs-lookup"><span data-stu-id="feceb-123">Never send data.</span></span>|
|<span data-ttu-id="feceb-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="feceb-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="feceb-125">4</span><span class="sxs-lookup"><span data-stu-id="feceb-125">4</span></span>|<span data-ttu-id="feceb-126">メッセージを表示せず、すべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="feceb-126">Send all data without prompting.</span></span>|





