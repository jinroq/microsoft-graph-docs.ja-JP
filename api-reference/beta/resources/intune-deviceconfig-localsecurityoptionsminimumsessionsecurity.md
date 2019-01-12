---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 822c996d788fd5edb5c92f876c725b771b051c15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952483"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="be08f-103">localSecurityOptionsMinimumSessionSecurity 列挙型</span><span class="sxs-lookup"><span data-stu-id="be08f-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="be08f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="be08f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be08f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be08f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="be08f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="be08f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="be08f-107">LocalSecurityOptionsMinimumSessionSecurity に指定できる値</span><span class="sxs-lookup"><span data-stu-id="be08f-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="be08f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="be08f-108">Members</span></span>
|<span data-ttu-id="be08f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="be08f-109">Member</span></span>|<span data-ttu-id="be08f-110">値</span><span class="sxs-lookup"><span data-stu-id="be08f-110">Value</span></span>|<span data-ttu-id="be08f-111">説明</span><span class="sxs-lookup"><span data-stu-id="be08f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be08f-112">none</span><span class="sxs-lookup"><span data-stu-id="be08f-112">none</span></span>|<span data-ttu-id="be08f-113">0</span><span class="sxs-lookup"><span data-stu-id="be08f-113">0</span></span>|<span data-ttu-id="be08f-114">LM と NTLM 応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="be08f-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="be08f-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="be08f-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="be08f-116">1</span><span class="sxs-lookup"><span data-stu-id="be08f-116">1</span></span>|<span data-ttu-id="be08f-117">ネゴシエートされた場合は、LM と NTLM を使用して NTLMv2 セッション セキュリティを送信します。</span><span class="sxs-lookup"><span data-stu-id="be08f-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="be08f-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="be08f-118">require128BitEncryption</span></span>|<span data-ttu-id="be08f-119">2</span><span class="sxs-lookup"><span data-stu-id="be08f-119">2</span></span>|<span data-ttu-id="be08f-120">LM と NTLM 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="be08f-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="be08f-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="be08f-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="be08f-122">3</span><span class="sxs-lookup"><span data-stu-id="be08f-122">3</span></span>|<span data-ttu-id="be08f-123">LM と NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="be08f-123">Send LM & NTLMv2 responses only</span></span>|





