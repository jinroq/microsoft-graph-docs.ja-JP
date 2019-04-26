---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: WIP 保護適用レベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1901059ef45141b0dc40d91dcbf4d9237cd6fc5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561174"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="07f6b-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="07f6b-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="07f6b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="07f6b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07f6b-105">WIP 保護適用レベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="07f6b-105">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="07f6b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="07f6b-106">Members</span></span>
|<span data-ttu-id="07f6b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="07f6b-107">Member</span></span>|<span data-ttu-id="07f6b-108">値</span><span class="sxs-lookup"><span data-stu-id="07f6b-108">Value</span></span>|<span data-ttu-id="07f6b-109">説明</span><span class="sxs-lookup"><span data-stu-id="07f6b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07f6b-110">noprotection</span><span class="sxs-lookup"><span data-stu-id="07f6b-110">noProtection</span></span>|<span data-ttu-id="07f6b-111">.0</span><span class="sxs-lookup"><span data-stu-id="07f6b-111">0</span></span>|<span data-ttu-id="07f6b-112">保護の適用なし</span><span class="sxs-lookup"><span data-stu-id="07f6b-112">No protection enforcement</span></span>|
|<span data-ttu-id="07f6b-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="07f6b-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="07f6b-114">1 </span><span class="sxs-lookup"><span data-stu-id="07f6b-114">1</span></span>|<span data-ttu-id="07f6b-115">暗号化と監査のみ</span><span class="sxs-lookup"><span data-stu-id="07f6b-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="07f6b-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="07f6b-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="07f6b-117">2 </span><span class="sxs-lookup"><span data-stu-id="07f6b-117">2</span></span>|<span data-ttu-id="07f6b-118">暗号化、監査、および確認</span><span class="sxs-lookup"><span data-stu-id="07f6b-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="07f6b-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="07f6b-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="07f6b-120">3 </span><span class="sxs-lookup"><span data-stu-id="07f6b-120">3</span></span>|<span data-ttu-id="07f6b-121">暗号化、監査、ブロック</span><span class="sxs-lookup"><span data-stu-id="07f6b-121">Encrypt, Audit and Block</span></span>|



