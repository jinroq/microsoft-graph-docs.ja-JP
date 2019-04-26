---
title: eapfastconfiguration 列挙型
description: eap-fast 構成で利用可能な設定。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7acf6ffbf7a93bc5002f7f81679fc789ab313e2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567145"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="bde8a-103">eapfastconfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="bde8a-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="bde8a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bde8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bde8a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bde8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bde8a-106">eap-fast 構成で利用可能な設定。</span><span class="sxs-lookup"><span data-stu-id="bde8a-106">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="bde8a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bde8a-107">Members</span></span>
|<span data-ttu-id="bde8a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bde8a-108">Member</span></span>|<span data-ttu-id="bde8a-109">値</span><span class="sxs-lookup"><span data-stu-id="bde8a-109">Value</span></span>|<span data-ttu-id="bde8a-110">説明</span><span class="sxs-lookup"><span data-stu-id="bde8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bde8a-111">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="bde8a-111">noProtectedAccessCredential</span></span>|<span data-ttu-id="bde8a-112">.0</span><span class="sxs-lookup"><span data-stu-id="bde8a-112">0</span></span>|<span data-ttu-id="bde8a-113">保護されたアクセス資格情報 (PAC) を使用せずに、eap-fast を使用します。</span><span class="sxs-lookup"><span data-stu-id="bde8a-113">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="bde8a-114">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="bde8a-114">useProtectedAccessCredential</span></span>|<span data-ttu-id="bde8a-115">1 </span><span class="sxs-lookup"><span data-stu-id="bde8a-115">1</span></span>|<span data-ttu-id="bde8a-116">保護されたアクセス資格情報 (PAC) を使用します。</span><span class="sxs-lookup"><span data-stu-id="bde8a-116">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="bde8a-117">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="bde8a-117">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="bde8a-118">2 </span><span class="sxs-lookup"><span data-stu-id="bde8a-118">2</span></span>|<span data-ttu-id="bde8a-119">保護されたアクセス資格情報 (pac) を使用し、pac をプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="bde8a-119">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="bde8a-120">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="bde8a-120">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="bde8a-121">3 </span><span class="sxs-lookup"><span data-stu-id="bde8a-121">3</span></span>|<span data-ttu-id="bde8a-122">保護されたアクセス資格情報 (pac) を使用し、pac をプロビジョニングして、匿名で行います。</span><span class="sxs-lookup"><span data-stu-id="bde8a-122">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





