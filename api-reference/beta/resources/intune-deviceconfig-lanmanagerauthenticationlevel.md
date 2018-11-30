---
title: lanManagerAuthenticationLevel 列挙型
description: LanManagerAuthenticationLevel に指定できる値
ms.openlocfilehash: 9fb8113c4953a0cabcecfbc5303b9f62f685d5ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066945"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="58fc0-103">lanManagerAuthenticationLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="58fc0-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="58fc0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58fc0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58fc0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58fc0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58fc0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="58fc0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58fc0-107">LanManagerAuthenticationLevel に指定できる値</span><span class="sxs-lookup"><span data-stu-id="58fc0-107">Possible values for LanManagerAuthenticationLevel</span></span>
## <a name="members"></a><span data-ttu-id="58fc0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="58fc0-108">Members</span></span>
|<span data-ttu-id="58fc0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="58fc0-109">Member</span></span>|<span data-ttu-id="58fc0-110">値</span><span class="sxs-lookup"><span data-stu-id="58fc0-110">Value</span></span>|<span data-ttu-id="58fc0-111">説明</span><span class="sxs-lookup"><span data-stu-id="58fc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58fc0-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="58fc0-112">lmAndNltm</span></span>|<span data-ttu-id="58fc0-113">0</span><span class="sxs-lookup"><span data-stu-id="58fc0-113">0</span></span>|<span data-ttu-id="58fc0-114">LM と NTLM 応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="58fc0-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="58fc0-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="58fc0-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="58fc0-116">1</span><span class="sxs-lookup"><span data-stu-id="58fc0-116">1</span></span>|<span data-ttu-id="58fc0-117">ネゴシエートされた場合は、LM と NTLM を使用して NTLMv2 セッション セキュリティを送信します。</span><span class="sxs-lookup"><span data-stu-id="58fc0-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="58fc0-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="58fc0-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="58fc0-119">2</span><span class="sxs-lookup"><span data-stu-id="58fc0-119">2</span></span>|<span data-ttu-id="58fc0-120">LM と NTLM 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="58fc0-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="58fc0-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="58fc0-121">lmAndNtlmV2</span></span>|<span data-ttu-id="58fc0-122">3</span><span class="sxs-lookup"><span data-stu-id="58fc0-122">3</span></span>|<span data-ttu-id="58fc0-123">LM と NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="58fc0-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="58fc0-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="58fc0-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="58fc0-125">4</span><span class="sxs-lookup"><span data-stu-id="58fc0-125">4</span></span>|<span data-ttu-id="58fc0-126">LM と NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="58fc0-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="58fc0-127">LM を拒否します。</span><span class="sxs-lookup"><span data-stu-id="58fc0-127">Refuse LM</span></span>|
|<span data-ttu-id="58fc0-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="58fc0-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="58fc0-129">5</span><span class="sxs-lookup"><span data-stu-id="58fc0-129">5</span></span>|<span data-ttu-id="58fc0-130">LM と NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="58fc0-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="58fc0-131">LM と NTLM を拒否します。</span><span class="sxs-lookup"><span data-stu-id="58fc0-131">Refuse LM & NTLM</span></span>|





