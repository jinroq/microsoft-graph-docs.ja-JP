---
title: windowsInformationProtectionEnforcementLevel 列挙型
description: WIP 保護適用レベルに指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd2f1a31004afca7a8c26533bd848011c16fef92
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967862"
---
# <a name="windowsinformationprotectionenforcementlevel-enum-type"></a><span data-ttu-id="c5c9f-103">windowsInformationProtectionEnforcementLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="c5c9f-103">windowsInformationProtectionEnforcementLevel enum type</span></span>

> <span data-ttu-id="c5c9f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5c9f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5c9f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5c9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5c9f-106">WIP 保護適用レベルに指定できる値</span><span class="sxs-lookup"><span data-stu-id="c5c9f-106">Possible values for WIP Protection enforcement levels</span></span>

## <a name="members"></a><span data-ttu-id="c5c9f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c5c9f-107">Members</span></span>
|<span data-ttu-id="c5c9f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c5c9f-108">Member</span></span>|<span data-ttu-id="c5c9f-109">値</span><span class="sxs-lookup"><span data-stu-id="c5c9f-109">Value</span></span>|<span data-ttu-id="c5c9f-110">説明</span><span class="sxs-lookup"><span data-stu-id="c5c9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5c9f-111">noProtection</span><span class="sxs-lookup"><span data-stu-id="c5c9f-111">noProtection</span></span>|<span data-ttu-id="c5c9f-112">.0</span><span class="sxs-lookup"><span data-stu-id="c5c9f-112">0</span></span>|<span data-ttu-id="c5c9f-113">保護の適用なし</span><span class="sxs-lookup"><span data-stu-id="c5c9f-113">No protection enforcement</span></span>|
|<span data-ttu-id="c5c9f-114">encryptAndAuditOnly</span><span class="sxs-lookup"><span data-stu-id="c5c9f-114">encryptAndAuditOnly</span></span>|<span data-ttu-id="c5c9f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c5c9f-115">1</span></span>|<span data-ttu-id="c5c9f-116">暗号化と監査のみ</span><span class="sxs-lookup"><span data-stu-id="c5c9f-116">Encrypt and Audit only</span></span>|
|<span data-ttu-id="c5c9f-117">encryptAuditAndPrompt</span><span class="sxs-lookup"><span data-stu-id="c5c9f-117">encryptAuditAndPrompt</span></span>|<span data-ttu-id="c5c9f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c5c9f-118">2</span></span>|<span data-ttu-id="c5c9f-119">暗号化、監査、および確認</span><span class="sxs-lookup"><span data-stu-id="c5c9f-119">Encrypt, Audit and Prompt</span></span>|
|<span data-ttu-id="c5c9f-120">encryptAuditAndBlock</span><span class="sxs-lookup"><span data-stu-id="c5c9f-120">encryptAuditAndBlock</span></span>|<span data-ttu-id="c5c9f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="c5c9f-121">3</span></span>|<span data-ttu-id="c5c9f-122">暗号化、監査、ブロック</span><span class="sxs-lookup"><span data-stu-id="c5c9f-122">Encrypt, Audit and Block</span></span>|





