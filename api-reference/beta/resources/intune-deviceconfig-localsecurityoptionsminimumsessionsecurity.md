---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac7ebd94f791372b4bd7b74189204a7b8a4d0360
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989295"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="5d720-103">localSecurityOptionsMinimumSessionSecurity 列挙型</span><span class="sxs-lookup"><span data-stu-id="5d720-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="5d720-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d720-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d720-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5d720-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d720-106">LocalSecurityOptionsMinimumSessionSecurity に指定できる値</span><span class="sxs-lookup"><span data-stu-id="5d720-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="5d720-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5d720-107">Members</span></span>
|<span data-ttu-id="5d720-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5d720-108">Member</span></span>|<span data-ttu-id="5d720-109">値</span><span class="sxs-lookup"><span data-stu-id="5d720-109">Value</span></span>|<span data-ttu-id="5d720-110">説明</span><span class="sxs-lookup"><span data-stu-id="5d720-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d720-111">none</span><span class="sxs-lookup"><span data-stu-id="5d720-111">none</span></span>|<span data-ttu-id="5d720-112">.0</span><span class="sxs-lookup"><span data-stu-id="5d720-112">0</span></span>|<span data-ttu-id="5d720-113">LM & NTLM 応答を送信する</span><span class="sxs-lookup"><span data-stu-id="5d720-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="5d720-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="5d720-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="5d720-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5d720-115">1</span></span>|<span data-ttu-id="5d720-116">LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する</span><span class="sxs-lookup"><span data-stu-id="5d720-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="5d720-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="5d720-117">require128BitEncryption</span></span>|<span data-ttu-id="5d720-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5d720-118">2</span></span>|<span data-ttu-id="5d720-119">LM & NTLM 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="5d720-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="5d720-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="5d720-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="5d720-121">1/3</span><span class="sxs-lookup"><span data-stu-id="5d720-121">3</span></span>|<span data-ttu-id="5d720-122">LM & NTLMv2 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="5d720-122">Send LM & NTLMv2 responses only</span></span>|





