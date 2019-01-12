---
title: eapFastConfiguration 列挙型
description: EAP-FAST 構成の使用可能な設定です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 65165929d388ed57f2651a0d277996e56d2f046e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954457"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="0797e-103">eapFastConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="0797e-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="0797e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0797e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0797e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0797e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0797e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0797e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0797e-107">EAP-FAST 構成の使用可能な設定です。</span><span class="sxs-lookup"><span data-stu-id="0797e-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="0797e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0797e-108">Members</span></span>
|<span data-ttu-id="0797e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0797e-109">Member</span></span>|<span data-ttu-id="0797e-110">値</span><span class="sxs-lookup"><span data-stu-id="0797e-110">Value</span></span>|<span data-ttu-id="0797e-111">説明</span><span class="sxs-lookup"><span data-stu-id="0797e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0797e-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="0797e-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="0797e-113">0</span><span class="sxs-lookup"><span data-stu-id="0797e-113">0</span></span>|<span data-ttu-id="0797e-114">EAP-FAST クリデンシャル (PAC) の保護されたアクセスなしを使用します。</span><span class="sxs-lookup"><span data-stu-id="0797e-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="0797e-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="0797e-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="0797e-116">1</span><span class="sxs-lookup"><span data-stu-id="0797e-116">1</span></span>|<span data-ttu-id="0797e-117">保護されたアクセス クリデンシャル (PAC) をを利用します。</span><span class="sxs-lookup"><span data-stu-id="0797e-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="0797e-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="0797e-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="0797e-119">2</span><span class="sxs-lookup"><span data-stu-id="0797e-119">2</span></span>|<span data-ttu-id="0797e-120">使用してアクセスを保護するクリデンシャル (PAC) と PAC. を提供します。</span><span class="sxs-lookup"><span data-stu-id="0797e-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="0797e-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="0797e-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="0797e-122">3</span><span class="sxs-lookup"><span data-stu-id="0797e-122">3</span></span>|<span data-ttu-id="0797e-123">保護されたアクセスの資格情報 (PAC)、PAC のプロビジョニングを使用して実行し、匿名で。</span><span class="sxs-lookup"><span data-stu-id="0797e-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





