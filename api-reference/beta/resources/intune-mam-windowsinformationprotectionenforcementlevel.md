---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed087465d05ba91bcdc1f8cff7fec0aba567420a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913409"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="07961-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="07961-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="07961-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07961-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07961-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07961-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07961-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="07961-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07961-107">仕掛品の保護の実施のレベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="07961-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="07961-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="07961-108">Members</span></span>
|<span data-ttu-id="07961-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="07961-109">Member</span></span>|<span data-ttu-id="07961-110">値</span><span class="sxs-lookup"><span data-stu-id="07961-110">Value</span></span>|<span data-ttu-id="07961-111">説明</span><span class="sxs-lookup"><span data-stu-id="07961-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07961-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="07961-112">noProtection</span></span>|<span data-ttu-id="07961-113">0</span><span class="sxs-lookup"><span data-stu-id="07961-113">0</span></span>|<span data-ttu-id="07961-114">なしの保護の実施</span><span class="sxs-lookup"><span data-stu-id="07961-114">No protection enforcement</span></span>|
|<span data-ttu-id="07961-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="07961-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="07961-116">1</span><span class="sxs-lookup"><span data-stu-id="07961-116">1</span></span>|<span data-ttu-id="07961-117">暗号化し、[監査のみ]</span><span class="sxs-lookup"><span data-stu-id="07961-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="07961-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="07961-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="07961-119">2</span><span class="sxs-lookup"><span data-stu-id="07961-119">2</span></span>|<span data-ttu-id="07961-120">暗号化、監査、およびメッセージを表示</span><span class="sxs-lookup"><span data-stu-id="07961-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="07961-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="07961-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="07961-122">3</span><span class="sxs-lookup"><span data-stu-id="07961-122">3</span></span>|<span data-ttu-id="07961-123">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="07961-123">Encrypt, Audit and Block</span></span>|





