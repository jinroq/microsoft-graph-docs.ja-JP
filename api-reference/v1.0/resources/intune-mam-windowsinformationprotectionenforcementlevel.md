---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b3ffff4e1d78ed8796f4b5be8768db99d6b4ae3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820189"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="1d033-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="1d033-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="1d033-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d033-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d033-105">仕掛品の保護の実施のレベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="1d033-105">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="1d033-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1d033-106">Members</span></span>
|<span data-ttu-id="1d033-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1d033-107">Member</span></span>|<span data-ttu-id="1d033-108">値</span><span class="sxs-lookup"><span data-stu-id="1d033-108">Value</span></span>|<span data-ttu-id="1d033-109">説明</span><span class="sxs-lookup"><span data-stu-id="1d033-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d033-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="1d033-110">noProtection</span></span>|<span data-ttu-id="1d033-111">0</span><span class="sxs-lookup"><span data-stu-id="1d033-111">0</span></span>|<span data-ttu-id="1d033-112">なしの保護の実施</span><span class="sxs-lookup"><span data-stu-id="1d033-112">No protection enforcement</span></span>|
|<span data-ttu-id="1d033-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="1d033-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="1d033-114">1</span><span class="sxs-lookup"><span data-stu-id="1d033-114">1</span></span>|<span data-ttu-id="1d033-115">暗号化し、[監査のみ]</span><span class="sxs-lookup"><span data-stu-id="1d033-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="1d033-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="1d033-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="1d033-117">2</span><span class="sxs-lookup"><span data-stu-id="1d033-117">2</span></span>|<span data-ttu-id="1d033-118">暗号化、監査、およびメッセージを表示</span><span class="sxs-lookup"><span data-stu-id="1d033-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="1d033-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="1d033-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="1d033-120">3</span><span class="sxs-lookup"><span data-stu-id="1d033-120">3</span></span>|<span data-ttu-id="1d033-121">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="1d033-121">Encrypt, Audit and Block</span></span>|



