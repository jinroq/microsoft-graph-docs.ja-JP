---
title: lanManagerAuthenticationLevel 列挙型
description: LanManagerAuthenticationLevel に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ade139765c9a362cd0c9f9365af0026c51ecb4ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356726"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="4df10-103">lanManagerAuthenticationLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="4df10-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="4df10-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4df10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4df10-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4df10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4df10-106">LanManagerAuthenticationLevel に指定できる値</span><span class="sxs-lookup"><span data-stu-id="4df10-106">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="4df10-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4df10-107">Members</span></span>
|<span data-ttu-id="4df10-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4df10-108">Member</span></span>|<span data-ttu-id="4df10-109">値</span><span class="sxs-lookup"><span data-stu-id="4df10-109">Value</span></span>|<span data-ttu-id="4df10-110">説明</span><span class="sxs-lookup"><span data-stu-id="4df10-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4df10-111">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="4df10-111">lmAndNltm</span></span>|<span data-ttu-id="4df10-112">.0</span><span class="sxs-lookup"><span data-stu-id="4df10-112">0</span></span>|<span data-ttu-id="4df10-113">LM & NTLM 応答を送信する</span><span class="sxs-lookup"><span data-stu-id="4df10-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="4df10-114">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="4df10-114">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="4df10-115">1-d</span><span class="sxs-lookup"><span data-stu-id="4df10-115">1</span></span>|<span data-ttu-id="4df10-116">LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する</span><span class="sxs-lookup"><span data-stu-id="4df10-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="4df10-117">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="4df10-117">lmAndNtlmOnly</span></span>|<span data-ttu-id="4df10-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4df10-118">2</span></span>|<span data-ttu-id="4df10-119">LM & NTLM 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="4df10-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="4df10-120">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="4df10-120">lmAndNtlmV2</span></span>|<span data-ttu-id="4df10-121">1/3</span><span class="sxs-lookup"><span data-stu-id="4df10-121">3</span></span>|<span data-ttu-id="4df10-122">LM & NTLMv2 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="4df10-122">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="4df10-123">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="4df10-123">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="4df10-124">2/4</span><span class="sxs-lookup"><span data-stu-id="4df10-124">4</span></span>|<span data-ttu-id="4df10-125">LM & NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="4df10-125">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="4df10-126">LM を拒否する</span><span class="sxs-lookup"><span data-stu-id="4df10-126">Refuse LM</span></span>|
|<span data-ttu-id="4df10-127">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="4df10-127">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="4df10-128">5</span><span class="sxs-lookup"><span data-stu-id="4df10-128">5</span></span>|<span data-ttu-id="4df10-129">LM & NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="4df10-129">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="4df10-130">NTLM & の LM を拒否する</span><span class="sxs-lookup"><span data-stu-id="4df10-130">Refuse LM & NTLM</span></span>|



