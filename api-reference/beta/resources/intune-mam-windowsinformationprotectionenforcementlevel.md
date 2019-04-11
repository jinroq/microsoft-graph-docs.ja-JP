---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: WIP 保護適用レベルに指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac5a360bebfc60dbaf4315be5e4e189f91c1f2b8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801618"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="0c085-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="0c085-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="0c085-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c085-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c085-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c085-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c085-106">WIP 保護適用レベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="0c085-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="0c085-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0c085-107">Members</span></span>
|<span data-ttu-id="0c085-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0c085-108">Member</span></span>|<span data-ttu-id="0c085-109">値</span><span class="sxs-lookup"><span data-stu-id="0c085-109">Value</span></span>|<span data-ttu-id="0c085-110">説明</span><span class="sxs-lookup"><span data-stu-id="0c085-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c085-111">noprotection</span><span class="sxs-lookup"><span data-stu-id="0c085-111">noProtection</span></span>|<span data-ttu-id="0c085-112">.0</span><span class="sxs-lookup"><span data-stu-id="0c085-112">0</span></span>|<span data-ttu-id="0c085-113">保護の適用なし</span><span class="sxs-lookup"><span data-stu-id="0c085-113">No protection enforcement</span></span>|
|<span data-ttu-id="0c085-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="0c085-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="0c085-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0c085-115">1</span></span>|<span data-ttu-id="0c085-116">暗号化と監査のみ</span><span class="sxs-lookup"><span data-stu-id="0c085-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="0c085-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="0c085-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="0c085-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0c085-118">2</span></span>|<span data-ttu-id="0c085-119">暗号化、監査、および確認</span><span class="sxs-lookup"><span data-stu-id="0c085-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="0c085-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="0c085-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="0c085-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0c085-121">3</span></span>|<span data-ttu-id="0c085-122">暗号化、監査、ブロック</span><span class="sxs-lookup"><span data-stu-id="0c085-122">Encrypt, Audit and Block</span></span>|





