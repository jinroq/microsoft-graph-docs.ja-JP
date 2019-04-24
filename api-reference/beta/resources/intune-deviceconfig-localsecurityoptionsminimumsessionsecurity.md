---
title: localsecurityoptionsminimumsessionsecurity 列挙型
description: localsecurityoptionsminimumsessionsecurity に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a087c9d99164ce5c830b2d40022d7ddd99736547
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460654"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="3901d-103">localsecurityoptionsminimumsessionsecurity 列挙型</span><span class="sxs-lookup"><span data-stu-id="3901d-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="3901d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3901d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3901d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3901d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3901d-106">localsecurityoptionsminimumsessionsecurity に指定できる値</span><span class="sxs-lookup"><span data-stu-id="3901d-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="3901d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3901d-107">Members</span></span>
|<span data-ttu-id="3901d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3901d-108">Member</span></span>|<span data-ttu-id="3901d-109">値</span><span class="sxs-lookup"><span data-stu-id="3901d-109">Value</span></span>|<span data-ttu-id="3901d-110">説明</span><span class="sxs-lookup"><span data-stu-id="3901d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3901d-111">なし</span><span class="sxs-lookup"><span data-stu-id="3901d-111">none</span></span>|<span data-ttu-id="3901d-112">.0</span><span class="sxs-lookup"><span data-stu-id="3901d-112">0</span></span>|<span data-ttu-id="3901d-113">LM & NTLM 応答の送信</span><span class="sxs-lookup"><span data-stu-id="3901d-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="3901d-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="3901d-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="3901d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3901d-115">1</span></span>|<span data-ttu-id="3901d-116">LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する</span><span class="sxs-lookup"><span data-stu-id="3901d-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="3901d-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="3901d-117">require128BitEncryption</span></span>|<span data-ttu-id="3901d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3901d-118">2</span></span>|<span data-ttu-id="3901d-119">LM & NTLM 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="3901d-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="3901d-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="3901d-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="3901d-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3901d-121">3</span></span>|<span data-ttu-id="3901d-122">LM & NTLMv2 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="3901d-122">Send LM & NTLMv2 responses only</span></span>|





