---
title: defenderPromptForSampleSubmission 列挙型
description: ユーザーにサンプル送信のプロンプトを表示するために使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aa8b9b636ffeaeab90e076e8a4c537df275c246e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031892"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="02696-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="02696-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="02696-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="02696-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02696-105">ユーザーにサンプル送信のプロンプトを表示するために使用できる値。</span><span class="sxs-lookup"><span data-stu-id="02696-105">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="02696-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="02696-106">Members</span></span>
|<span data-ttu-id="02696-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="02696-107">Member</span></span>|<span data-ttu-id="02696-108">値</span><span class="sxs-lookup"><span data-stu-id="02696-108">Value</span></span>|<span data-ttu-id="02696-109">説明</span><span class="sxs-lookup"><span data-stu-id="02696-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02696-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="02696-110">userDefined</span></span>|<span data-ttu-id="02696-111">.0</span><span class="sxs-lookup"><span data-stu-id="02696-111">0</span></span>|<span data-ttu-id="02696-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="02696-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="02696-113">Always プロンプト</span><span class="sxs-lookup"><span data-stu-id="02696-113">alwaysPrompt</span></span>|<span data-ttu-id="02696-114">1-d</span><span class="sxs-lookup"><span data-stu-id="02696-114">1</span></span>|<span data-ttu-id="02696-115">常にプロンプトを表示します。</span><span class="sxs-lookup"><span data-stu-id="02696-115">Always prompt.</span></span>|
|<span data-ttu-id="02696-116">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="02696-116">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="02696-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="02696-117">2</span></span>|<span data-ttu-id="02696-118">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="02696-118">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="02696-119">neverSendData</span><span class="sxs-lookup"><span data-stu-id="02696-119">neverSendData</span></span>|<span data-ttu-id="02696-120">1/3</span><span class="sxs-lookup"><span data-stu-id="02696-120">3</span></span>|<span data-ttu-id="02696-121">データを送信しません。</span><span class="sxs-lookup"><span data-stu-id="02696-121">Never send data.</span></span>|
|<span data-ttu-id="02696-122">Sendalldataメッセージを表示しない</span><span class="sxs-lookup"><span data-stu-id="02696-122">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="02696-123">2/4</span><span class="sxs-lookup"><span data-stu-id="02696-123">4</span></span>|<span data-ttu-id="02696-124">メッセージを表示せずにすべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="02696-124">Send all data without prompting.</span></span>|



