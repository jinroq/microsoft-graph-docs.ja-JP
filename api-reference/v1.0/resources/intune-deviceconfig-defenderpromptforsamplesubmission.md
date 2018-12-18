---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
author: tfitzmac
ms.openlocfilehash: 36a9790b669c588205824be60d350d2750637b15
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312748"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="1d711-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="1d711-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="1d711-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d711-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d711-105">サンプル提出用のユーザーにメッセージを表示可能な値です。</span><span class="sxs-lookup"><span data-stu-id="1d711-105">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="1d711-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1d711-106">Members</span></span>
|<span data-ttu-id="1d711-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1d711-107">Member</span></span>|<span data-ttu-id="1d711-108">値</span><span class="sxs-lookup"><span data-stu-id="1d711-108">Value</span></span>|<span data-ttu-id="1d711-109">説明</span><span class="sxs-lookup"><span data-stu-id="1d711-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d711-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="1d711-110">userDefined</span></span>|<span data-ttu-id="1d711-111">0</span><span class="sxs-lookup"><span data-stu-id="1d711-111">0</span></span>|<span data-ttu-id="1d711-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="1d711-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="1d711-113">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="1d711-113">alwaysPrompt</span></span>|<span data-ttu-id="1d711-114">1</span><span class="sxs-lookup"><span data-stu-id="1d711-114">1</span></span>|<span data-ttu-id="1d711-115">常にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="1d711-115">Always prompt.</span></span>|
|<span data-ttu-id="1d711-116">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="1d711-116">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="1d711-117">2</span><span class="sxs-lookup"><span data-stu-id="1d711-117">2</span></span>|<span data-ttu-id="1d711-118">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="1d711-118">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="1d711-119">neverSendData</span><span class="sxs-lookup"><span data-stu-id="1d711-119">neverSendData</span></span>|<span data-ttu-id="1d711-120">3</span><span class="sxs-lookup"><span data-stu-id="1d711-120">3</span></span>|<span data-ttu-id="1d711-121">データを送信しないでください。</span><span class="sxs-lookup"><span data-stu-id="1d711-121">Never send data.</span></span>|
|<span data-ttu-id="1d711-122">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="1d711-122">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="1d711-123">4</span><span class="sxs-lookup"><span data-stu-id="1d711-123">4</span></span>|<span data-ttu-id="1d711-124">メッセージを表示せず、すべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="1d711-124">Send all data without prompting.</span></span>|



