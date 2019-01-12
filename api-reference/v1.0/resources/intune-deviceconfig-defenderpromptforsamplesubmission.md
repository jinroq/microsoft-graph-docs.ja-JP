---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e103916bd55e6c2d505a85c379b80962ab9a0cac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928088"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="19650-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="19650-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="19650-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="19650-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19650-105">サンプル提出用のユーザーにメッセージを表示可能な値です。</span><span class="sxs-lookup"><span data-stu-id="19650-105">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="19650-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="19650-106">Members</span></span>
|<span data-ttu-id="19650-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="19650-107">Member</span></span>|<span data-ttu-id="19650-108">値</span><span class="sxs-lookup"><span data-stu-id="19650-108">Value</span></span>|<span data-ttu-id="19650-109">説明</span><span class="sxs-lookup"><span data-stu-id="19650-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19650-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="19650-110">userDefined</span></span>|<span data-ttu-id="19650-111">0</span><span class="sxs-lookup"><span data-stu-id="19650-111">0</span></span>|<span data-ttu-id="19650-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="19650-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="19650-113">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="19650-113">alwaysPrompt</span></span>|<span data-ttu-id="19650-114">1</span><span class="sxs-lookup"><span data-stu-id="19650-114">1</span></span>|<span data-ttu-id="19650-115">常にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="19650-115">Always prompt.</span></span>|
|<span data-ttu-id="19650-116">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="19650-116">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="19650-117">2</span><span class="sxs-lookup"><span data-stu-id="19650-117">2</span></span>|<span data-ttu-id="19650-118">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="19650-118">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="19650-119">neverSendData</span><span class="sxs-lookup"><span data-stu-id="19650-119">neverSendData</span></span>|<span data-ttu-id="19650-120">3</span><span class="sxs-lookup"><span data-stu-id="19650-120">3</span></span>|<span data-ttu-id="19650-121">データを送信しないでください。</span><span class="sxs-lookup"><span data-stu-id="19650-121">Never send data.</span></span>|
|<span data-ttu-id="19650-122">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="19650-122">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="19650-123">4</span><span class="sxs-lookup"><span data-stu-id="19650-123">4</span></span>|<span data-ttu-id="19650-124">メッセージを表示せず、すべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="19650-124">Send all data without prompting.</span></span>|



