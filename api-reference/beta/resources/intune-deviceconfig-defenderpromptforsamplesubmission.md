---
title: defenderPromptForSampleSubmission 列挙型
description: ユーザーにサンプル送信のプロンプトを表示するために使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c81fe62d7ed2696b233b8684c665f7cf8341fbcd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778377"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="06de5-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="06de5-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="06de5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06de5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06de5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06de5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06de5-106">ユーザーにサンプル送信のプロンプトを表示するために使用できる値。</span><span class="sxs-lookup"><span data-stu-id="06de5-106">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="06de5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="06de5-107">Members</span></span>
|<span data-ttu-id="06de5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="06de5-108">Member</span></span>|<span data-ttu-id="06de5-109">値</span><span class="sxs-lookup"><span data-stu-id="06de5-109">Value</span></span>|<span data-ttu-id="06de5-110">説明</span><span class="sxs-lookup"><span data-stu-id="06de5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06de5-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="06de5-111">userDefined</span></span>|<span data-ttu-id="06de5-112">.0</span><span class="sxs-lookup"><span data-stu-id="06de5-112">0</span></span>|<span data-ttu-id="06de5-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="06de5-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="06de5-114">always プロンプト</span><span class="sxs-lookup"><span data-stu-id="06de5-114">alwaysPrompt</span></span>|<span data-ttu-id="06de5-115">1-d</span><span class="sxs-lookup"><span data-stu-id="06de5-115">1</span></span>|<span data-ttu-id="06de5-116">常にプロンプトを表示します。</span><span class="sxs-lookup"><span data-stu-id="06de5-116">Always prompt.</span></span>|
|<span data-ttu-id="06de5-117">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="06de5-117">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="06de5-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="06de5-118">2</span></span>|<span data-ttu-id="06de5-119">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="06de5-119">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="06de5-120">neverSendData</span><span class="sxs-lookup"><span data-stu-id="06de5-120">neverSendData</span></span>|<span data-ttu-id="06de5-121">1/3</span><span class="sxs-lookup"><span data-stu-id="06de5-121">3</span></span>|<span data-ttu-id="06de5-122">データを送信しません。</span><span class="sxs-lookup"><span data-stu-id="06de5-122">Never send data.</span></span>|
|<span data-ttu-id="06de5-123">sendalldataメッセージを表示しない</span><span class="sxs-lookup"><span data-stu-id="06de5-123">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="06de5-124">2/4</span><span class="sxs-lookup"><span data-stu-id="06de5-124">4</span></span>|<span data-ttu-id="06de5-125">メッセージを表示せずにすべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="06de5-125">Send all data without prompting.</span></span>|





