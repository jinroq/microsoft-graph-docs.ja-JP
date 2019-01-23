---
title: defenderPromptForSampleSubmission 列挙型
description: サンプル提出用のユーザーにメッセージを表示可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b706c0086791543a5cbb13d26ae1d86a2e3b1760
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403316"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="9138a-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="9138a-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="9138a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9138a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9138a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9138a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9138a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9138a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9138a-107">サンプル提出用のユーザーにメッセージを表示可能な値です。</span><span class="sxs-lookup"><span data-stu-id="9138a-107">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="9138a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9138a-108">Members</span></span>
|<span data-ttu-id="9138a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="9138a-109">Member</span></span>|<span data-ttu-id="9138a-110">値</span><span class="sxs-lookup"><span data-stu-id="9138a-110">Value</span></span>|<span data-ttu-id="9138a-111">説明</span><span class="sxs-lookup"><span data-stu-id="9138a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9138a-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="9138a-112">userDefined</span></span>|<span data-ttu-id="9138a-113">0</span><span class="sxs-lookup"><span data-stu-id="9138a-113">0</span></span>|<span data-ttu-id="9138a-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="9138a-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="9138a-115">alwaysPrompt</span><span class="sxs-lookup"><span data-stu-id="9138a-115">alwaysPrompt</span></span>|<span data-ttu-id="9138a-116">1</span><span class="sxs-lookup"><span data-stu-id="9138a-116">1</span></span>|<span data-ttu-id="9138a-117">常にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="9138a-117">Always prompt.</span></span>|
|<span data-ttu-id="9138a-118">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="9138a-118">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="9138a-119">2</span><span class="sxs-lookup"><span data-stu-id="9138a-119">2</span></span>|<span data-ttu-id="9138a-120">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="9138a-120">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="9138a-121">neverSendData</span><span class="sxs-lookup"><span data-stu-id="9138a-121">neverSendData</span></span>|<span data-ttu-id="9138a-122">3</span><span class="sxs-lookup"><span data-stu-id="9138a-122">3</span></span>|<span data-ttu-id="9138a-123">データを送信しないでください。</span><span class="sxs-lookup"><span data-stu-id="9138a-123">Never send data.</span></span>|
|<span data-ttu-id="9138a-124">sendAllDataWithoutPrompting</span><span class="sxs-lookup"><span data-stu-id="9138a-124">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="9138a-125">4</span><span class="sxs-lookup"><span data-stu-id="9138a-125">4</span></span>|<span data-ttu-id="9138a-126">メッセージを表示せず、すべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="9138a-126">Send all data without prompting.</span></span>|




