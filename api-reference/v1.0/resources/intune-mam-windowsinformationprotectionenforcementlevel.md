---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4661c80655defe85f27ac8259a961955552f7021
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964173"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="6697f-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="6697f-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="6697f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6697f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6697f-105">仕掛品の保護の実施のレベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="6697f-105">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="6697f-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="6697f-106">Members</span></span>
|<span data-ttu-id="6697f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6697f-107">Member</span></span>|<span data-ttu-id="6697f-108">値</span><span class="sxs-lookup"><span data-stu-id="6697f-108">Value</span></span>|<span data-ttu-id="6697f-109">説明</span><span class="sxs-lookup"><span data-stu-id="6697f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6697f-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="6697f-110">noProtection</span></span>|<span data-ttu-id="6697f-111">0</span><span class="sxs-lookup"><span data-stu-id="6697f-111">0</span></span>|<span data-ttu-id="6697f-112">なしの保護の実施</span><span class="sxs-lookup"><span data-stu-id="6697f-112">No protection enforcement</span></span>|
|<span data-ttu-id="6697f-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="6697f-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="6697f-114">1</span><span class="sxs-lookup"><span data-stu-id="6697f-114">1</span></span>|<span data-ttu-id="6697f-115">暗号化し、[監査のみ]</span><span class="sxs-lookup"><span data-stu-id="6697f-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="6697f-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="6697f-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="6697f-117">2</span><span class="sxs-lookup"><span data-stu-id="6697f-117">2</span></span>|<span data-ttu-id="6697f-118">暗号化、監査、およびメッセージを表示</span><span class="sxs-lookup"><span data-stu-id="6697f-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="6697f-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="6697f-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="6697f-120">3</span><span class="sxs-lookup"><span data-stu-id="6697f-120">3</span></span>|<span data-ttu-id="6697f-121">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="6697f-121">Encrypt, Audit and Block</span></span>|



