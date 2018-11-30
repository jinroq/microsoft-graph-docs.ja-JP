---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
ms.openlocfilehash: 7b4d7cee068fe45317b4fdf9c4e9372cae293e32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020656"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="97e9c-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="97e9c-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="97e9c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="97e9c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97e9c-105">サンプル提出用のユーザーにメッセージを表示可能な値です。</span><span class="sxs-lookup"><span data-stu-id="97e9c-105">Possible values for prompting user for samples submission.</span></span>
## <a name="members"></a><span data-ttu-id="97e9c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="97e9c-106">Members</span></span>
|<span data-ttu-id="97e9c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="97e9c-107">Member</span></span>|<span data-ttu-id="97e9c-108">値</span><span class="sxs-lookup"><span data-stu-id="97e9c-108">Value</span></span>|<span data-ttu-id="97e9c-109">説明</span><span class="sxs-lookup"><span data-stu-id="97e9c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97e9c-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="97e9c-110">userDefined</span></span>|<span data-ttu-id="97e9c-111">0</span><span class="sxs-lookup"><span data-stu-id="97e9c-111">0</span></span>|<span data-ttu-id="97e9c-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="97e9c-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="97e9c-113">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="97e9c-113">alwaysPrompt</span></span>|<span data-ttu-id="97e9c-114">1</span><span class="sxs-lookup"><span data-stu-id="97e9c-114">1</span></span>|<span data-ttu-id="97e9c-115">常にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="97e9c-115">Always prompt.</span></span>|
|<span data-ttu-id="97e9c-116">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="97e9c-116">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="97e9c-117">2</span><span class="sxs-lookup"><span data-stu-id="97e9c-117">2</span></span>|<span data-ttu-id="97e9c-118">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="97e9c-118">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="97e9c-119">neverSendData</span><span class="sxs-lookup"><span data-stu-id="97e9c-119">neverSendData</span></span>|<span data-ttu-id="97e9c-120">3</span><span class="sxs-lookup"><span data-stu-id="97e9c-120">3</span></span>|<span data-ttu-id="97e9c-121">データを送信しないでください。</span><span class="sxs-lookup"><span data-stu-id="97e9c-121">Never send data.</span></span>|
|<span data-ttu-id="97e9c-122">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="97e9c-122">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="97e9c-123">4</span><span class="sxs-lookup"><span data-stu-id="97e9c-123">4</span></span>|<span data-ttu-id="97e9c-124">メッセージを表示せず、すべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="97e9c-124">Send all data without prompting.</span></span>|



