---
title: eapfastconfiguration 列挙型
description: eap-fast 構成で利用可能な設定。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0d8a250b2272ae8b8287f9869697633493b116f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173571"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="9a7dd-103">eapfastconfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="9a7dd-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="9a7dd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a7dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a7dd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9a7dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a7dd-106">eap-fast 構成で利用可能な設定。</span><span class="sxs-lookup"><span data-stu-id="9a7dd-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="9a7dd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9a7dd-107">Members</span></span>
|<span data-ttu-id="9a7dd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9a7dd-108">Member</span></span>|<span data-ttu-id="9a7dd-109">値</span><span class="sxs-lookup"><span data-stu-id="9a7dd-109">Value</span></span>|<span data-ttu-id="9a7dd-110">説明</span><span class="sxs-lookup"><span data-stu-id="9a7dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a7dd-111">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="9a7dd-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="9a7dd-112">.0</span><span class="sxs-lookup"><span data-stu-id="9a7dd-112">0</span></span>|<span data-ttu-id="9a7dd-113">保護されたアクセス資格情報 (PAC) を使用せずに、eap-fast を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a7dd-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="9a7dd-114">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="9a7dd-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="9a7dd-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9a7dd-115">1</span></span>|<span data-ttu-id="9a7dd-116">保護されたアクセス資格情報 (PAC) を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a7dd-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="9a7dd-117">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="9a7dd-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="9a7dd-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9a7dd-118">2</span></span>|<span data-ttu-id="9a7dd-119">保護されたアクセス資格情報 (pac) を使用し、pac をプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="9a7dd-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="9a7dd-120">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="9a7dd-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="9a7dd-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9a7dd-121">3</span></span>|<span data-ttu-id="9a7dd-122">保護されたアクセス資格情報 (pac) を使用し、pac をプロビジョニングして、匿名で行います。</span><span class="sxs-lookup"><span data-stu-id="9a7dd-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|




