---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: 仕掛品の保護の実施のレベルに指定できる値
author: tfitzmac
ms.openlocfilehash: 84f60f0e4f59206d420219e8547160c85202f9cf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313266"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="727ec-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="727ec-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="727ec-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="727ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="727ec-105">仕掛品の保護の実施のレベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="727ec-105">Possible values for WIP Protection enforcement levels</span></span>
## <a name="members"></a><span data-ttu-id="727ec-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="727ec-106">Members</span></span>
|<span data-ttu-id="727ec-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="727ec-107">Member</span></span>|<span data-ttu-id="727ec-108">値</span><span class="sxs-lookup"><span data-stu-id="727ec-108">Value</span></span>|<span data-ttu-id="727ec-109">説明</span><span class="sxs-lookup"><span data-stu-id="727ec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="727ec-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="727ec-110">noProtection</span></span>|<span data-ttu-id="727ec-111">0</span><span class="sxs-lookup"><span data-stu-id="727ec-111">0</span></span>|<span data-ttu-id="727ec-112">なしの保護の実施</span><span class="sxs-lookup"><span data-stu-id="727ec-112">No protection enforcement</span></span>|
|<span data-ttu-id="727ec-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="727ec-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="727ec-114">1</span><span class="sxs-lookup"><span data-stu-id="727ec-114">1</span></span>|<span data-ttu-id="727ec-115">暗号化し、[監査のみ]</span><span class="sxs-lookup"><span data-stu-id="727ec-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="727ec-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="727ec-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="727ec-117">2</span><span class="sxs-lookup"><span data-stu-id="727ec-117">2</span></span>|<span data-ttu-id="727ec-118">暗号化、監査、およびメッセージを表示</span><span class="sxs-lookup"><span data-stu-id="727ec-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="727ec-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="727ec-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="727ec-120">3</span><span class="sxs-lookup"><span data-stu-id="727ec-120">3</span></span>|<span data-ttu-id="727ec-121">暗号化、監査、およびブロック</span><span class="sxs-lookup"><span data-stu-id="727ec-121">Encrypt, Audit and Block</span></span>|



