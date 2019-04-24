---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: WIP 保護適用レベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac5a360bebfc60dbaf4315be5e4e189f91c1f2b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522140"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="c3bbd-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="c3bbd-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="c3bbd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3bbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3bbd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3bbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3bbd-106">WIP 保護適用レベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="c3bbd-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="c3bbd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c3bbd-107">Members</span></span>
|<span data-ttu-id="c3bbd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c3bbd-108">Member</span></span>|<span data-ttu-id="c3bbd-109">値</span><span class="sxs-lookup"><span data-stu-id="c3bbd-109">Value</span></span>|<span data-ttu-id="c3bbd-110">説明</span><span class="sxs-lookup"><span data-stu-id="c3bbd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3bbd-111">noprotection</span><span class="sxs-lookup"><span data-stu-id="c3bbd-111">noProtection</span></span>|<span data-ttu-id="c3bbd-112">.0</span><span class="sxs-lookup"><span data-stu-id="c3bbd-112">0</span></span>|<span data-ttu-id="c3bbd-113">保護の適用なし</span><span class="sxs-lookup"><span data-stu-id="c3bbd-113">No protection enforcement</span></span>|
|<span data-ttu-id="c3bbd-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="c3bbd-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="c3bbd-115">1 </span><span class="sxs-lookup"><span data-stu-id="c3bbd-115">1</span></span>|<span data-ttu-id="c3bbd-116">暗号化と監査のみ</span><span class="sxs-lookup"><span data-stu-id="c3bbd-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="c3bbd-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="c3bbd-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="c3bbd-118">2 </span><span class="sxs-lookup"><span data-stu-id="c3bbd-118">2</span></span>|<span data-ttu-id="c3bbd-119">暗号化、監査、および確認</span><span class="sxs-lookup"><span data-stu-id="c3bbd-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="c3bbd-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="c3bbd-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="c3bbd-121">3 </span><span class="sxs-lookup"><span data-stu-id="c3bbd-121">3</span></span>|<span data-ttu-id="c3bbd-122">暗号化、監査、ブロック</span><span class="sxs-lookup"><span data-stu-id="c3bbd-122">Encrypt, Audit and Block</span></span>|





