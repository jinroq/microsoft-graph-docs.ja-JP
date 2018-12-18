---
title: eapFastConfiguration 列挙型
description: EAP-FAST 構成の使用可能な設定です。
author: tfitzmac
ms.openlocfilehash: ba84adb86e9910df47bd236fd2bd348cbc9c8e6f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326363"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="bdb27-103">eapFastConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="bdb27-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="bdb27-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bdb27-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdb27-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdb27-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdb27-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bdb27-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdb27-107">EAP-FAST 構成の使用可能な設定です。</span><span class="sxs-lookup"><span data-stu-id="bdb27-107">Available settings for EAP-FAST Configuration.</span></span>
## <a name="members"></a><span data-ttu-id="bdb27-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bdb27-108">Members</span></span>
|<span data-ttu-id="bdb27-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="bdb27-109">Member</span></span>|<span data-ttu-id="bdb27-110">値</span><span class="sxs-lookup"><span data-stu-id="bdb27-110">Value</span></span>|<span data-ttu-id="bdb27-111">説明</span><span class="sxs-lookup"><span data-stu-id="bdb27-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdb27-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="bdb27-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="bdb27-113">0</span><span class="sxs-lookup"><span data-stu-id="bdb27-113">0</span></span>|<span data-ttu-id="bdb27-114">EAP-FAST クリデンシャル (PAC) の保護されたアクセスなしを使用します。</span><span class="sxs-lookup"><span data-stu-id="bdb27-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="bdb27-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="bdb27-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="bdb27-116">1</span><span class="sxs-lookup"><span data-stu-id="bdb27-116">1</span></span>|<span data-ttu-id="bdb27-117">保護されたアクセス クリデンシャル (PAC) をを利用します。</span><span class="sxs-lookup"><span data-stu-id="bdb27-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="bdb27-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="bdb27-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="bdb27-119">2</span><span class="sxs-lookup"><span data-stu-id="bdb27-119">2</span></span>|<span data-ttu-id="bdb27-120">使用してアクセスを保護するクリデンシャル (PAC) と PAC. を提供します。</span><span class="sxs-lookup"><span data-stu-id="bdb27-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="bdb27-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="bdb27-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="bdb27-122">3</span><span class="sxs-lookup"><span data-stu-id="bdb27-122">3</span></span>|<span data-ttu-id="bdb27-123">保護されたアクセスの資格情報 (PAC)、PAC のプロビジョニングを使用して実行し、匿名で。</span><span class="sxs-lookup"><span data-stu-id="bdb27-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|





