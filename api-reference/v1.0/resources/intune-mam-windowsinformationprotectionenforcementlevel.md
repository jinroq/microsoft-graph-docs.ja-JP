---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: WIP 保護適用レベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 99229243502d9dcf1c96139aa2173081a4ea314e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037710"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="d40a0-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="d40a0-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="d40a0-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d40a0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d40a0-105">WIP 保護適用レベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="d40a0-105">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="d40a0-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d40a0-106">Members</span></span>
|<span data-ttu-id="d40a0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d40a0-107">Member</span></span>|<span data-ttu-id="d40a0-108">値</span><span class="sxs-lookup"><span data-stu-id="d40a0-108">Value</span></span>|<span data-ttu-id="d40a0-109">説明</span><span class="sxs-lookup"><span data-stu-id="d40a0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d40a0-110">noProtection</span><span class="sxs-lookup"><span data-stu-id="d40a0-110">noProtection</span></span>|<span data-ttu-id="d40a0-111">.0</span><span class="sxs-lookup"><span data-stu-id="d40a0-111">0</span></span>|<span data-ttu-id="d40a0-112">保護の適用なし</span><span class="sxs-lookup"><span data-stu-id="d40a0-112">No protection enforcement</span></span>|
|<span data-ttu-id="d40a0-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="d40a0-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="d40a0-114">1-d</span><span class="sxs-lookup"><span data-stu-id="d40a0-114">1</span></span>|<span data-ttu-id="d40a0-115">暗号化と監査のみ</span><span class="sxs-lookup"><span data-stu-id="d40a0-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="d40a0-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="d40a0-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="d40a0-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d40a0-117">2</span></span>|<span data-ttu-id="d40a0-118">暗号化、監査、および確認</span><span class="sxs-lookup"><span data-stu-id="d40a0-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="d40a0-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="d40a0-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="d40a0-120">1/3</span><span class="sxs-lookup"><span data-stu-id="d40a0-120">3</span></span>|<span data-ttu-id="d40a0-121">暗号化、監査、ブロック</span><span class="sxs-lookup"><span data-stu-id="d40a0-121">Encrypt, Audit and Block</span></span>|



