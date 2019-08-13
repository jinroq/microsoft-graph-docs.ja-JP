---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8dc6a96f5dda3cdba9ea3a57507bef4f32edc5a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325527"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="eb9fd-103">localSecurityOptionsMinimumSessionSecurity 列挙型</span><span class="sxs-lookup"><span data-stu-id="eb9fd-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="eb9fd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb9fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb9fd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb9fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb9fd-106">LocalSecurityOptionsMinimumSessionSecurity に指定できる値</span><span class="sxs-lookup"><span data-stu-id="eb9fd-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="eb9fd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="eb9fd-107">Members</span></span>
|<span data-ttu-id="eb9fd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="eb9fd-108">Member</span></span>|<span data-ttu-id="eb9fd-109">値</span><span class="sxs-lookup"><span data-stu-id="eb9fd-109">Value</span></span>|<span data-ttu-id="eb9fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="eb9fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb9fd-111">none</span><span class="sxs-lookup"><span data-stu-id="eb9fd-111">none</span></span>|<span data-ttu-id="eb9fd-112">.0</span><span class="sxs-lookup"><span data-stu-id="eb9fd-112">0</span></span>|<span data-ttu-id="eb9fd-113">LM & NTLM 応答を送信する</span><span class="sxs-lookup"><span data-stu-id="eb9fd-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="eb9fd-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="eb9fd-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="eb9fd-115">1-d</span><span class="sxs-lookup"><span data-stu-id="eb9fd-115">1</span></span>|<span data-ttu-id="eb9fd-116">LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する</span><span class="sxs-lookup"><span data-stu-id="eb9fd-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="eb9fd-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="eb9fd-117">require128BitEncryption</span></span>|<span data-ttu-id="eb9fd-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="eb9fd-118">2</span></span>|<span data-ttu-id="eb9fd-119">LM & NTLM 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="eb9fd-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="eb9fd-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="eb9fd-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="eb9fd-121">1/3</span><span class="sxs-lookup"><span data-stu-id="eb9fd-121">3</span></span>|<span data-ttu-id="eb9fd-122">LM & NTLMv2 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="eb9fd-122">Send LM & NTLMv2 responses only</span></span>|



