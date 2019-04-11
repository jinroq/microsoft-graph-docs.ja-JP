---
title: lanmanagerauthenticationlevel 列挙型
description: lanmanagerauthenticationlevel に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3b93f229661de3e2fbb28f764288983b2fd83bb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801247"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="88ba6-103">lanmanagerauthenticationlevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="88ba6-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="88ba6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88ba6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88ba6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88ba6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88ba6-106">lanmanagerauthenticationlevel に指定できる値</span><span class="sxs-lookup"><span data-stu-id="88ba6-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="88ba6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="88ba6-107">Members</span></span>
|<span data-ttu-id="88ba6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="88ba6-108">Member</span></span>|<span data-ttu-id="88ba6-109">値</span><span class="sxs-lookup"><span data-stu-id="88ba6-109">Value</span></span>|<span data-ttu-id="88ba6-110">説明</span><span class="sxs-lookup"><span data-stu-id="88ba6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88ba6-111">lmandnltm</span><span class="sxs-lookup"><span data-stu-id="88ba6-111">lmAndNltm</span></span>|<span data-ttu-id="88ba6-112">.0</span><span class="sxs-lookup"><span data-stu-id="88ba6-112">0</span></span>|<span data-ttu-id="88ba6-113">LM & NTLM 応答の送信</span><span class="sxs-lookup"><span data-stu-id="88ba6-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="88ba6-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="88ba6-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="88ba6-115">1-d</span><span class="sxs-lookup"><span data-stu-id="88ba6-115">1</span></span>|<span data-ttu-id="88ba6-116">LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する</span><span class="sxs-lookup"><span data-stu-id="88ba6-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="88ba6-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="88ba6-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="88ba6-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="88ba6-118">2</span></span>|<span data-ttu-id="88ba6-119">LM & NTLM 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="88ba6-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="88ba6-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="88ba6-120">lmAndNtlmV2</span></span>|<span data-ttu-id="88ba6-121">1/3</span><span class="sxs-lookup"><span data-stu-id="88ba6-121">3</span></span>|<span data-ttu-id="88ba6-122">LM & NTLMv2 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="88ba6-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="88ba6-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="88ba6-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="88ba6-124">2/4</span><span class="sxs-lookup"><span data-stu-id="88ba6-124">4</span></span>|<span data-ttu-id="88ba6-125">LM & NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="88ba6-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="88ba6-126">lm を拒否する</span><span class="sxs-lookup"><span data-stu-id="88ba6-126">Refuse LM</span></span>|
|<span data-ttu-id="88ba6-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="88ba6-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="88ba6-128">5</span><span class="sxs-lookup"><span data-stu-id="88ba6-128">5</span></span>|<span data-ttu-id="88ba6-129">LM & NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="88ba6-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="88ba6-130">lm & NTLM を拒否する</span><span class="sxs-lookup"><span data-stu-id="88ba6-130">Refuse LM & NTLM</span></span>|





