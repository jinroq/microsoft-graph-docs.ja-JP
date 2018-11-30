---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
ms.openlocfilehash: 969c7d6576c613f5214bfc3b8a5a1ad36722f0df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072332"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="85580-103">localSecurityOptionsMinimumSessionSecurity 列挙型</span><span class="sxs-lookup"><span data-stu-id="85580-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="85580-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="85580-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85580-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85580-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85580-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="85580-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85580-107">LocalSecurityOptionsMinimumSessionSecurity に指定できる値</span><span class="sxs-lookup"><span data-stu-id="85580-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>
## <a name="members"></a><span data-ttu-id="85580-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="85580-108">Members</span></span>
|<span data-ttu-id="85580-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="85580-109">Member</span></span>|<span data-ttu-id="85580-110">値</span><span class="sxs-lookup"><span data-stu-id="85580-110">Value</span></span>|<span data-ttu-id="85580-111">説明</span><span class="sxs-lookup"><span data-stu-id="85580-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85580-112">none</span><span class="sxs-lookup"><span data-stu-id="85580-112">none</span></span>|<span data-ttu-id="85580-113">0</span><span class="sxs-lookup"><span data-stu-id="85580-113">0</span></span>|<span data-ttu-id="85580-114">LM と NTLM 応答を送信します。</span><span class="sxs-lookup"><span data-stu-id="85580-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="85580-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="85580-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="85580-116">1</span><span class="sxs-lookup"><span data-stu-id="85580-116">1</span></span>|<span data-ttu-id="85580-117">ネゴシエートされた場合は、LM と NTLM を使用して NTLMv2 セッション セキュリティを送信します。</span><span class="sxs-lookup"><span data-stu-id="85580-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="85580-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="85580-118">require128BitEncryption</span></span>|<span data-ttu-id="85580-119">2</span><span class="sxs-lookup"><span data-stu-id="85580-119">2</span></span>|<span data-ttu-id="85580-120">LM と NTLM 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="85580-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="85580-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="85580-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="85580-122">3</span><span class="sxs-lookup"><span data-stu-id="85580-122">3</span></span>|<span data-ttu-id="85580-123">LM と NTLMv2 応答のみを送信します。</span><span class="sxs-lookup"><span data-stu-id="85580-123">Send LM & NTLMv2 responses only</span></span>|





