---
title: defenderPromptForSampleSubmission 列挙型
description: ユーザーにサンプル送信のプロンプトを表示するために使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fa3fb4f98f20b705c5905eb5fc0f07833815e228
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970921"
---
# <a name="defenderpromptforsamplesubmission-enum-type"></a><span data-ttu-id="29ddb-103">defenderPromptForSampleSubmission 列挙型</span><span class="sxs-lookup"><span data-stu-id="29ddb-103">defenderPromptForSampleSubmission enum type</span></span>

> <span data-ttu-id="29ddb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29ddb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29ddb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29ddb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29ddb-106">ユーザーにサンプル送信のプロンプトを表示するために使用できる値。</span><span class="sxs-lookup"><span data-stu-id="29ddb-106">Possible values for prompting user for samples submission.</span></span>

## <a name="members"></a><span data-ttu-id="29ddb-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="29ddb-107">Members</span></span>
|<span data-ttu-id="29ddb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="29ddb-108">Member</span></span>|<span data-ttu-id="29ddb-109">値</span><span class="sxs-lookup"><span data-stu-id="29ddb-109">Value</span></span>|<span data-ttu-id="29ddb-110">説明</span><span class="sxs-lookup"><span data-stu-id="29ddb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29ddb-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="29ddb-111">userDefined</span></span>|<span data-ttu-id="29ddb-112">.0</span><span class="sxs-lookup"><span data-stu-id="29ddb-112">0</span></span>|<span data-ttu-id="29ddb-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="29ddb-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="29ddb-114">Always プロンプト</span><span class="sxs-lookup"><span data-stu-id="29ddb-114">alwaysPrompt</span></span>|<span data-ttu-id="29ddb-115">1-d</span><span class="sxs-lookup"><span data-stu-id="29ddb-115">1</span></span>|<span data-ttu-id="29ddb-116">常にプロンプトを表示します。</span><span class="sxs-lookup"><span data-stu-id="29ddb-116">Always prompt.</span></span>|
|<span data-ttu-id="29ddb-117">promptBeforeSendingPersonalData</span><span class="sxs-lookup"><span data-stu-id="29ddb-117">promptBeforeSendingPersonalData</span></span>|<span data-ttu-id="29ddb-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="29ddb-118">2</span></span>|<span data-ttu-id="29ddb-119">個人データを送信する前にメッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="29ddb-119">Prompt before sending personal data.</span></span>|
|<span data-ttu-id="29ddb-120">neverSendData</span><span class="sxs-lookup"><span data-stu-id="29ddb-120">neverSendData</span></span>|<span data-ttu-id="29ddb-121">1/3</span><span class="sxs-lookup"><span data-stu-id="29ddb-121">3</span></span>|<span data-ttu-id="29ddb-122">データを送信しません。</span><span class="sxs-lookup"><span data-stu-id="29ddb-122">Never send data.</span></span>|
|<span data-ttu-id="29ddb-123">Sendalldataメッセージを表示しない</span><span class="sxs-lookup"><span data-stu-id="29ddb-123">sendAllDataWithoutPrompting</span></span>|<span data-ttu-id="29ddb-124">2/4</span><span class="sxs-lookup"><span data-stu-id="29ddb-124">4</span></span>|<span data-ttu-id="29ddb-125">メッセージを表示せずにすべてのデータを送信します。</span><span class="sxs-lookup"><span data-stu-id="29ddb-125">Send all data without prompting.</span></span>|





