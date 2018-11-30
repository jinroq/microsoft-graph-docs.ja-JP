---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
ms.openlocfilehash: 5d27923c53dbae0aaeebc6bd664f0cd7f6bd9e8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024161"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="8a1e1-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="8a1e1-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="8a1e1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a1e1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a1e1-105">仕掛品の保護の実施のレベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="8a1e1-105">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="8a1e1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a1e1-106">Members</span></span>
|<span data-ttu-id="8a1e1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a1e1-107">Member</span></span>|<span data-ttu-id="8a1e1-108">値</span><span class="sxs-lookup"><span data-stu-id="8a1e1-108">Value</span></span>|<span data-ttu-id="8a1e1-109">説明</span><span class="sxs-lookup"><span data-stu-id="8a1e1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a1e1-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="8a1e1-110">noProtection</span></span>|<span data-ttu-id="8a1e1-111">0</span><span class="sxs-lookup"><span data-stu-id="8a1e1-111">0</span></span>|<span data-ttu-id="8a1e1-112">なしの保護の実施</span><span class="sxs-lookup"><span data-stu-id="8a1e1-112">No protection enforcement</span></span>|
|<span data-ttu-id="8a1e1-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="8a1e1-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="8a1e1-114">1</span><span class="sxs-lookup"><span data-stu-id="8a1e1-114">1</span></span>|<span data-ttu-id="8a1e1-115">暗号化し、[監査のみ]</span><span class="sxs-lookup"><span data-stu-id="8a1e1-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="8a1e1-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="8a1e1-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="8a1e1-117">2</span><span class="sxs-lookup"><span data-stu-id="8a1e1-117">2</span></span>|<span data-ttu-id="8a1e1-118">暗号化、監査、およびメッセージを表示</span><span class="sxs-lookup"><span data-stu-id="8a1e1-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="8a1e1-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="8a1e1-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="8a1e1-120">3</span><span class="sxs-lookup"><span data-stu-id="8a1e1-120">3</span></span>|<span data-ttu-id="8a1e1-121">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="8a1e1-121">Encrypt, Audit and Block</span></span>|



