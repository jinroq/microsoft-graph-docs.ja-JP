---
title: eapFastConfiguration 列挙型
description: EAP-FAST 構成で利用可能な設定。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca19e48f07d7bdb2859af9924cd391a9dbdfdf3f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989890"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="3da4d-103">eapFastConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="3da4d-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="3da4d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3da4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3da4d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3da4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3da4d-106">EAP-FAST 構成で利用可能な設定。</span><span class="sxs-lookup"><span data-stu-id="3da4d-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="3da4d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3da4d-107">Members</span></span>
|<span data-ttu-id="3da4d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3da4d-108">Member</span></span>|<span data-ttu-id="3da4d-109">値</span><span class="sxs-lookup"><span data-stu-id="3da4d-109">Value</span></span>|<span data-ttu-id="3da4d-110">説明</span><span class="sxs-lookup"><span data-stu-id="3da4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3da4d-111">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="3da4d-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="3da4d-112">.0</span><span class="sxs-lookup"><span data-stu-id="3da4d-112">0</span></span>|<span data-ttu-id="3da4d-113">保護されたアクセス資格情報 (PAC) を使用せずに、EAP-FAST を使用します。</span><span class="sxs-lookup"><span data-stu-id="3da4d-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="3da4d-114">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="3da4d-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="3da4d-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3da4d-115">1</span></span>|<span data-ttu-id="3da4d-116">保護されたアクセス資格情報 (PAC) を使用します。</span><span class="sxs-lookup"><span data-stu-id="3da4d-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="3da4d-117">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="3da4d-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="3da4d-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3da4d-118">2</span></span>|<span data-ttu-id="3da4d-119">保護されたアクセス資格情報 (PAC) を使用し、PAC をプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="3da4d-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="3da4d-120">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="3da4d-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="3da4d-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3da4d-121">3</span></span>|<span data-ttu-id="3da4d-122">保護されたアクセス資格情報 (PAC) を使用し、PAC をプロビジョニングして、匿名で行います。</span><span class="sxs-lookup"><span data-stu-id="3da4d-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





