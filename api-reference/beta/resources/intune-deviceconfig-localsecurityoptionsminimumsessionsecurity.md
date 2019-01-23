---
title: localSecurityOptionsMinimumSessionSecurity 列挙型
description: LocalSecurityOptionsMinimumSessionSecurity に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c39f2bb6d0bab2aff09fc05bb0492e81102e1b7c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396085"
---
# <a name="localsecurityoptionsminimumsessionsecurity-enum-type"></a><span data-ttu-id="62be3-103">localSecurityOptionsMinimumSessionSecurity 列挙型</span><span class="sxs-lookup"><span data-stu-id="62be3-103">localSecurityOptionsMinimumSessionSecurity enum type</span></span>

> <span data-ttu-id="62be3-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="62be3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="62be3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62be3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62be3-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62be3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62be3-107">LocalSecurityOptionsMinimumSessionSecurity に指定できる値</span><span class="sxs-lookup"><span data-stu-id="62be3-107">Possible values for LocalSecurityOptionsMinimumSessionSecurity</span></span>

## <a name="members"></a><span data-ttu-id="62be3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="62be3-108">Members</span></span>
|<span data-ttu-id="62be3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="62be3-109">Member</span></span>|<span data-ttu-id="62be3-110">値</span><span class="sxs-lookup"><span data-stu-id="62be3-110">Value</span></span>|<span data-ttu-id="62be3-111">説明</span><span class="sxs-lookup"><span data-stu-id="62be3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62be3-112">none</span><span class="sxs-lookup"><span data-stu-id="62be3-112">none</span></span>|<span data-ttu-id="62be3-113">0</span><span class="sxs-lookup"><span data-stu-id="62be3-113">0</span></span>|<span data-ttu-id="62be3-114">NTLM 応答を送信するには、LM &</span><span class="sxs-lookup"><span data-stu-id="62be3-114">Send LM & NTLM responses</span></span>|
|<span data-ttu-id="62be3-115">requireNtmlV2SessionSecurity</span><span class="sxs-lookup"><span data-stu-id="62be3-115">requireNtmlV2SessionSecurity</span></span>|<span data-ttu-id="62be3-116">1</span><span class="sxs-lookup"><span data-stu-id="62be3-116">1</span></span>|<span data-ttu-id="62be3-117">LM NTLM の使用を & の NTLMv2 セッション セキュリティをネゴシエートされた場合に送信します。</span><span class="sxs-lookup"><span data-stu-id="62be3-117">Send LM & NTLM-use NTLMv2 session security if negotiated</span></span>|
|<span data-ttu-id="62be3-118">require128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="62be3-118">require128BitEncryption</span></span>|<span data-ttu-id="62be3-119">2</span><span class="sxs-lookup"><span data-stu-id="62be3-119">2</span></span>|<span data-ttu-id="62be3-120">NTLM 応答のみを送信するには、LM &</span><span class="sxs-lookup"><span data-stu-id="62be3-120">Send LM & NTLM responses only</span></span>|
|<span data-ttu-id="62be3-121">ntlmV2And128BitEncryption</span><span class="sxs-lookup"><span data-stu-id="62be3-121">ntlmV2And128BitEncryption</span></span>|<span data-ttu-id="62be3-122">3</span><span class="sxs-lookup"><span data-stu-id="62be3-122">3</span></span>|<span data-ttu-id="62be3-123">NTLMv2 応答のみを送信するには、LM &</span><span class="sxs-lookup"><span data-stu-id="62be3-123">Send LM & NTLMv2 responses only</span></span>|




