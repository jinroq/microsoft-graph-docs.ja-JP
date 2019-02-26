---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: WIP 保護適用レベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1901059ef45141b0dc40d91dcbf4d9237cd6fc5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254815"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="d6158-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="d6158-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="d6158-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d6158-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6158-105">WIP 保護適用レベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="d6158-105">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="d6158-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6158-106">Members</span></span>
|<span data-ttu-id="d6158-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6158-107">Member</span></span>|<span data-ttu-id="d6158-108">値</span><span class="sxs-lookup"><span data-stu-id="d6158-108">Value</span></span>|<span data-ttu-id="d6158-109">説明</span><span class="sxs-lookup"><span data-stu-id="d6158-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6158-110">noprotection</span><span class="sxs-lookup"><span data-stu-id="d6158-110">noProtection</span></span>|<span data-ttu-id="d6158-111">.0</span><span class="sxs-lookup"><span data-stu-id="d6158-111">0</span></span>|<span data-ttu-id="d6158-112">保護の適用なし</span><span class="sxs-lookup"><span data-stu-id="d6158-112">No protection enforcement</span></span>|
|<span data-ttu-id="d6158-113">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="d6158-113">encryptAndAuditOnly</span></span>|<span data-ttu-id="d6158-114">1-d</span><span class="sxs-lookup"><span data-stu-id="d6158-114">1</span></span>|<span data-ttu-id="d6158-115">暗号化と監査のみ</span><span class="sxs-lookup"><span data-stu-id="d6158-115">Encrypt and Audit only</span></span>|
|<span data-ttu-id="d6158-116">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="d6158-116">encryptAuditAndPrompt</span></span>|<span data-ttu-id="d6158-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d6158-117">2</span></span>|<span data-ttu-id="d6158-118">暗号化、監査、および確認</span><span class="sxs-lookup"><span data-stu-id="d6158-118">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="d6158-119">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="d6158-119">encryptAuditAndBlock</span></span>|<span data-ttu-id="d6158-120">1/3</span><span class="sxs-lookup"><span data-stu-id="d6158-120">3</span></span>|<span data-ttu-id="d6158-121">暗号化、監査、ブロック</span><span class="sxs-lookup"><span data-stu-id="d6158-121">Encrypt, Audit and Block</span></span>|



