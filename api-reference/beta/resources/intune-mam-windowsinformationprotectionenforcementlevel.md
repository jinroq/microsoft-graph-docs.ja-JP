---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
ms.openlocfilehash: a590132f80028af513d4244f49904267b3a85f50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070811"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="cee03-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="cee03-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="cee03-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cee03-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cee03-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cee03-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cee03-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cee03-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cee03-107">仕掛品の保護の実施のレベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="cee03-107">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="cee03-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="cee03-108">Members</span></span>
|<span data-ttu-id="cee03-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="cee03-109">Member</span></span>|<span data-ttu-id="cee03-110">値</span><span class="sxs-lookup"><span data-stu-id="cee03-110">Value</span></span>|<span data-ttu-id="cee03-111">説明</span><span class="sxs-lookup"><span data-stu-id="cee03-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee03-112">noProtection</span><span class="sxs-lookup"><span data-stu-id="cee03-112">noProtection</span></span>|<span data-ttu-id="cee03-113">0</span><span class="sxs-lookup"><span data-stu-id="cee03-113">0</span></span>|<span data-ttu-id="cee03-114">なしの保護の実施</span><span class="sxs-lookup"><span data-stu-id="cee03-114">No protection enforcement</span></span>|
|<span data-ttu-id="cee03-115">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="cee03-115">encryptAndAuditOnly</span></span>|<span data-ttu-id="cee03-116">1</span><span class="sxs-lookup"><span data-stu-id="cee03-116">1</span></span>|<span data-ttu-id="cee03-117">暗号化し、[監査のみ]</span><span class="sxs-lookup"><span data-stu-id="cee03-117">Encrypt and Audit only</span></span>|
|<span data-ttu-id="cee03-118">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="cee03-118">encryptAuditAndPrompt</span></span>|<span data-ttu-id="cee03-119">2</span><span class="sxs-lookup"><span data-stu-id="cee03-119">2</span></span>|<span data-ttu-id="cee03-120">暗号化、監査、およびメッセージを表示</span><span class="sxs-lookup"><span data-stu-id="cee03-120">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="cee03-121">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="cee03-121">encryptAuditAndBlock</span></span>|<span data-ttu-id="cee03-122">3</span><span class="sxs-lookup"><span data-stu-id="cee03-122">3</span></span>|<span data-ttu-id="cee03-123">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="cee03-123">Encrypt, Audit and Block</span></span>|





