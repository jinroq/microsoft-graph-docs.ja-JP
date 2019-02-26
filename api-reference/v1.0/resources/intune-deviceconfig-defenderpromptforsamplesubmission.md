---
title: defenderPromptForSampleSubmission 列挙型
description: ユーザーにサンプル送信のプロンプトを表示するために使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1df39da4989417a8e21e5d0dad61667354e28ed
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251042"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="55e67-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="55e67-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="55e67-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="55e67-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55e67-105">ユーザーにサンプル送信のプロンプトを表示するために使用できる値。</span><span class="sxs-lookup"><span data-stu-id="55e67-105">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="55e67-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="55e67-106">Members</span></span>
|<span data-ttu-id="55e67-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="55e67-107">Member</span></span>|<span data-ttu-id="55e67-108">値</span><span class="sxs-lookup"><span data-stu-id="55e67-108">Value</span></span>|<span data-ttu-id="55e67-109">説明</span><span class="sxs-lookup"><span data-stu-id="55e67-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55e67-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="55e67-110">userDefined</span></span>|<span data-ttu-id="55e67-111">.0</span><span class="sxs-lookup"><span data-stu-id="55e67-111">0</span></span>|<span data-ttu-id="55e67-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="55e67-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="55e67-113">always プロンプト</span><span class="sxs-lookup"><span data-stu-id="55e67-113">alwaysPrompt</span></span>|<span data-ttu-id="55e67-114">1-d</span><span class="sxs-lookup"><span data-stu-id="55e67-114">1</span></span>|<span data-ttu-id="55e67-115">常にプロンプトを表示します。</span><span class="sxs-lookup"><span data-stu-id="55e67-115">Always prompt.</span></span>|
|<span data-ttu-id="55e67-116">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="55e67-116">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="55e67-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="55e67-117">2</span></span>|<span data-ttu-id="55e67-118">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="55e67-118">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="55e67-119">neverSendData</span><span class="sxs-lookup"><span data-stu-id="55e67-119">neverSendData</span></span>|<span data-ttu-id="55e67-120">1/3</span><span class="sxs-lookup"><span data-stu-id="55e67-120">3</span></span>|<span data-ttu-id="55e67-121">データを送信しません。</span><span class="sxs-lookup"><span data-stu-id="55e67-121">Never send data.</span></span>|
|<span data-ttu-id="55e67-122">sendalldataメッセージを表示しない</span><span class="sxs-lookup"><span data-stu-id="55e67-122">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="55e67-123">2/4</span><span class="sxs-lookup"><span data-stu-id="55e67-123">4</span></span>|<span data-ttu-id="55e67-124">メッセージを表示せずにすべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="55e67-124">Send all data without prompting.</span></span>|



