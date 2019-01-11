---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fb6912e7d3bba42364849165cceb28050ddacfae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833237"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="072be-103">localSecurityOptionsMinimumSessionSecurity 列挙型</span><span class="sxs-lookup"><span data-stu-id="072be-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="072be-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="072be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="072be-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="072be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="072be-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="072be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="072be-107">LocalSecurityOptionsMinimumSessionSecurity に指定できる値</span><span class="sxs-lookup"><span data-stu-id="072be-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="072be-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="072be-108">Members</span></span>
|<span data-ttu-id="072be-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="072be-109">Member</span></span>|<span data-ttu-id="072be-110">値</span><span class="sxs-lookup"><span data-stu-id="072be-110">Value</span></span>|<span data-ttu-id="072be-111">説明</span><span class="sxs-lookup"><span data-stu-id="072be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="072be-112">none</span><span class="sxs-lookup"><span data-stu-id="072be-112">none</span></span>|<span data-ttu-id="072be-113">0</span><span class="sxs-lookup"><span data-stu-id="072be-113">0</span></span>|<span data-ttu-id="072be-114">LM と NTLM 応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="072be-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="072be-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="072be-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="072be-116">1</span><span class="sxs-lookup"><span data-stu-id="072be-116">1</span></span>|<span data-ttu-id="072be-117">ネゴシエートされた場合は、LM と NTLM を使用して NTLMv2 セッション セキュリティを送信します。</span><span class="sxs-lookup"><span data-stu-id="072be-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="072be-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="072be-118">require128BitEncryption</span></span>|<span data-ttu-id="072be-119">2</span><span class="sxs-lookup"><span data-stu-id="072be-119">2</span></span>|<span data-ttu-id="072be-120">LM と NTLM 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="072be-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="072be-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="072be-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="072be-122">3</span><span class="sxs-lookup"><span data-stu-id="072be-122">3</span></span>|<span data-ttu-id="072be-123">LM と NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="072be-123">Send LM & NTLMv2 responses only</span></span>|





