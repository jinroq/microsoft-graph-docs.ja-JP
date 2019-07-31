---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 182c375ae8e70e7190f9860a72d04e7f508bc61e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001034"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="bae03-103">localSecurityOptionsMinimumSessionSecurity 列挙型</span><span class="sxs-lookup"><span data-stu-id="bae03-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="bae03-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bae03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bae03-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bae03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bae03-106">LocalSecurityOptionsMinimumSessionSecurity に指定できる値</span><span class="sxs-lookup"><span data-stu-id="bae03-106">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="bae03-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bae03-107">Members</span></span>
|<span data-ttu-id="bae03-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bae03-108">Member</span></span>|<span data-ttu-id="bae03-109">値</span><span class="sxs-lookup"><span data-stu-id="bae03-109">Value</span></span>|<span data-ttu-id="bae03-110">説明</span><span class="sxs-lookup"><span data-stu-id="bae03-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bae03-111">none</span><span class="sxs-lookup"><span data-stu-id="bae03-111">none</span></span>|<span data-ttu-id="bae03-112">.0</span><span class="sxs-lookup"><span data-stu-id="bae03-112">0</span></span>|<span data-ttu-id="bae03-113">LM & NTLM 応答を送信する</span><span class="sxs-lookup"><span data-stu-id="bae03-113">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="bae03-114">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="bae03-114">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="bae03-115">1-d</span><span class="sxs-lookup"><span data-stu-id="bae03-115">1</span></span>|<span data-ttu-id="bae03-116">LM & NTLM を送信する-ネゴシエートされる場合は NTLMv2 セッションセキュリティを使用する</span><span class="sxs-lookup"><span data-stu-id="bae03-116">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="bae03-117">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="bae03-117">require128BitEncryption</span></span>|<span data-ttu-id="bae03-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="bae03-118">2</span></span>|<span data-ttu-id="bae03-119">LM & NTLM 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="bae03-119">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="bae03-120">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="bae03-120">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="bae03-121">1/3</span><span class="sxs-lookup"><span data-stu-id="bae03-121">3</span></span>|<span data-ttu-id="bae03-122">LM & NTLMv2 応答のみを送信する</span><span class="sxs-lookup"><span data-stu-id="bae03-122">Send LM & NTLMv2 responses only</span></span>|





