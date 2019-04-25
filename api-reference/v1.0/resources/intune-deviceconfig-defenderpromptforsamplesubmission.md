---
title: defenderPromptForSampleSubmission 列挙型
description: ユーザーにサンプル送信のプロンプトを表示するために使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1df39da4989417a8e21e5d0dad61667354e28ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534277"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="ed08b-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="ed08b-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="ed08b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ed08b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed08b-105">ユーザーにサンプル送信のプロンプトを表示するために使用できる値。</span><span class="sxs-lookup"><span data-stu-id="ed08b-105">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="ed08b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ed08b-106">Members</span></span>
|<span data-ttu-id="ed08b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ed08b-107">Member</span></span>|<span data-ttu-id="ed08b-108">値</span><span class="sxs-lookup"><span data-stu-id="ed08b-108">Value</span></span>|<span data-ttu-id="ed08b-109">説明</span><span class="sxs-lookup"><span data-stu-id="ed08b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed08b-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="ed08b-110">userDefined</span></span>|<span data-ttu-id="ed08b-111">.0</span><span class="sxs-lookup"><span data-stu-id="ed08b-111">0</span></span>|<span data-ttu-id="ed08b-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="ed08b-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ed08b-113">always プロンプト</span><span class="sxs-lookup"><span data-stu-id="ed08b-113">alwaysPrompt</span></span>|<span data-ttu-id="ed08b-114">1 </span><span class="sxs-lookup"><span data-stu-id="ed08b-114">1</span></span>|<span data-ttu-id="ed08b-115">常にプロンプトを表示します。</span><span class="sxs-lookup"><span data-stu-id="ed08b-115">Always prompt.</span></span>|
|<span data-ttu-id="ed08b-116">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="ed08b-116">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="ed08b-117">2 </span><span class="sxs-lookup"><span data-stu-id="ed08b-117">2</span></span>|<span data-ttu-id="ed08b-118">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="ed08b-118">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="ed08b-119">neverSendData</span><span class="sxs-lookup"><span data-stu-id="ed08b-119">neverSendData</span></span>|<span data-ttu-id="ed08b-120">3 </span><span class="sxs-lookup"><span data-stu-id="ed08b-120">3</span></span>|<span data-ttu-id="ed08b-121">データを送信しません。</span><span class="sxs-lookup"><span data-stu-id="ed08b-121">Never send data.</span></span>|
|<span data-ttu-id="ed08b-122">sendalldataメッセージを表示しない</span><span class="sxs-lookup"><span data-stu-id="ed08b-122">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="ed08b-123">4 </span><span class="sxs-lookup"><span data-stu-id="ed08b-123">4</span></span>|<span data-ttu-id="ed08b-124">メッセージを表示せずにすべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="ed08b-124">Send all data without prompting.</span></span>|



