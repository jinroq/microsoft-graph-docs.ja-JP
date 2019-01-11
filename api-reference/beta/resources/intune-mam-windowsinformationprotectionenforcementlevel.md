---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5097682172281ece366a8f0389c314e2fb630190
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868370"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="c71b5-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="c71b5-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="c71b5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c71b5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c71b5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c71b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c71b5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c71b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c71b5-107">仕掛品の保護の実施のレベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="c71b5-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="c71b5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c71b5-108">Members</span></span>
|<span data-ttu-id="c71b5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c71b5-109">Member</span></span>|<span data-ttu-id="c71b5-110">値</span><span class="sxs-lookup"><span data-stu-id="c71b5-110">Value</span></span>|<span data-ttu-id="c71b5-111">説明</span><span class="sxs-lookup"><span data-stu-id="c71b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c71b5-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="c71b5-112">noProtection</span></span>|<span data-ttu-id="c71b5-113">0</span><span class="sxs-lookup"><span data-stu-id="c71b5-113">0</span></span>|<span data-ttu-id="c71b5-114">なしの保護の実施</span><span class="sxs-lookup"><span data-stu-id="c71b5-114">No protection enforcement</span></span>|
|<span data-ttu-id="c71b5-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="c71b5-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="c71b5-116">1</span><span class="sxs-lookup"><span data-stu-id="c71b5-116">1</span></span>|<span data-ttu-id="c71b5-117">暗号化し、[監査のみ]</span><span class="sxs-lookup"><span data-stu-id="c71b5-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="c71b5-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="c71b5-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="c71b5-119">2</span><span class="sxs-lookup"><span data-stu-id="c71b5-119">2</span></span>|<span data-ttu-id="c71b5-120">暗号化、監査、およびメッセージを表示</span><span class="sxs-lookup"><span data-stu-id="c71b5-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="c71b5-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="c71b5-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="c71b5-122">3</span><span class="sxs-lookup"><span data-stu-id="c71b5-122">3</span></span>|<span data-ttu-id="c71b5-123">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="c71b5-123">Encrypt, Audit and Block</span></span>|





