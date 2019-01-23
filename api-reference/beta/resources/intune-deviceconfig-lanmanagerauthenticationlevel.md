---
title: lanManagerAuthenticationLevel 列挙型
description: LanManagerAuthenticationLevel に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6e8c7b3df6f515d3dad0d7619b6c0b755ad799d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397457"
---
# <a name="lanmanagerauthenticationlevel-enum-type"></a><span data-ttu-id="7dbc5-103">lanManagerAuthenticationLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="7dbc5-103">lanManagerAuthenticationLevel enum type</span></span>

> <span data-ttu-id="7dbc5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7dbc5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7dbc5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dbc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7dbc5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7dbc5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dbc5-107">LanManagerAuthenticationLevel に指定できる値</span><span class="sxs-lookup"><span data-stu-id="7dbc5-107">Possible values for LanManagerAuthenticationLevel</span></span>

## <a name="members"></a><span data-ttu-id="7dbc5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7dbc5-108">Members</span></span>
|<span data-ttu-id="7dbc5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7dbc5-109">Member</span></span>|<span data-ttu-id="7dbc5-110">値</span><span class="sxs-lookup"><span data-stu-id="7dbc5-110">Value</span></span>|<span data-ttu-id="7dbc5-111">説明</span><span class="sxs-lookup"><span data-stu-id="7dbc5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dbc5-112">lmAndNltm</span><span class="sxs-lookup"><span data-stu-id="7dbc5-112">lmAndNltm</span></span>|<span data-ttu-id="7dbc5-113">0</span><span class="sxs-lookup"><span data-stu-id="7dbc5-113">0</span></span>|<span data-ttu-id="7dbc5-114">NTLM 応答を送信するには、LM &</span><span class="sxs-lookup"><span data-stu-id="7dbc5-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="7dbc5-115">lmNtlmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="7dbc5-115">lmNtlmAndNtlmV2</span></span>|<span data-ttu-id="7dbc5-116">1</span><span class="sxs-lookup"><span data-stu-id="7dbc5-116">1</span></span>|<span data-ttu-id="7dbc5-117">LM NTLM の使用を & の NTLMv2 セッション セキュリティをネゴシエートされた場合に送信します。</span><span class="sxs-lookup"><span data-stu-id="7dbc5-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="7dbc5-118">lmAndNtlmOnly</span><span class="sxs-lookup"><span data-stu-id="7dbc5-118">lmAndNtlmOnly</span></span>|<span data-ttu-id="7dbc5-119">2</span><span class="sxs-lookup"><span data-stu-id="7dbc5-119">2</span></span>|<span data-ttu-id="7dbc5-120">NTLM 応答のみを送信するには、LM &</span><span class="sxs-lookup"><span data-stu-id="7dbc5-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="7dbc5-121">lmAndNtlmV2</span><span class="sxs-lookup"><span data-stu-id="7dbc5-121">lmAndNtlmV2</span></span>|<span data-ttu-id="7dbc5-122">3</span><span class="sxs-lookup"><span data-stu-id="7dbc5-122">3</span></span>|<span data-ttu-id="7dbc5-123">NTLMv2 応答のみを送信するには、LM &</span><span class="sxs-lookup"><span data-stu-id="7dbc5-123">Send LM & NTLMv2 responses only</span></span>|
|<span data-ttu-id="7dbc5-124">lmNtlmV2AndNotLm</span><span class="sxs-lookup"><span data-stu-id="7dbc5-124">lmNtlmV2AndNotLm</span></span>|<span data-ttu-id="7dbc5-125">4</span><span class="sxs-lookup"><span data-stu-id="7dbc5-125">4</span></span>|<span data-ttu-id="7dbc5-126">LM & NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="7dbc5-126">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="7dbc5-127">LM を拒否します。</span><span class="sxs-lookup"><span data-stu-id="7dbc5-127">Refuse LM</span></span>|
|<span data-ttu-id="7dbc5-128">lmNtlmV2AndNotLmOrNtm</span><span class="sxs-lookup"><span data-stu-id="7dbc5-128">lmNtlmV2AndNotLmOrNtm</span></span>|<span data-ttu-id="7dbc5-129">5</span><span class="sxs-lookup"><span data-stu-id="7dbc5-129">5</span></span>|<span data-ttu-id="7dbc5-130">LM & NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="7dbc5-130">Send LM & NTLMv2 responses only.</span></span> <span data-ttu-id="7dbc5-131">LM & NTLM を拒否します。</span><span class="sxs-lookup"><span data-stu-id="7dbc5-131">Refuse LM & NTLM</span></span>|




