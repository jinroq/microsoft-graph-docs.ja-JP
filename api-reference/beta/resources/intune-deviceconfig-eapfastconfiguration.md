---
title: eapFastConfiguration 列挙型
description: EAP-FAST 構成の使用可能な設定です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa2c3c3a4cf0bc245ea7c9fbc4294d69215deee
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399389"
---
# <a name="eapfastconfiguration-enum-type"></a><span data-ttu-id="e0a84-103">eapFastConfiguration 列挙型</span><span class="sxs-lookup"><span data-stu-id="e0a84-103">eapFastConfiguration enum type</span></span>

> <span data-ttu-id="e0a84-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0a84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e0a84-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0a84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0a84-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0a84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0a84-107">EAP-FAST 構成の使用可能な設定です。</span><span class="sxs-lookup"><span data-stu-id="e0a84-107">Available settings for EAP-FAST Configuration.</span></span>

## <a name="members"></a><span data-ttu-id="e0a84-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0a84-108">Members</span></span>
|<span data-ttu-id="e0a84-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0a84-109">Member</span></span>|<span data-ttu-id="e0a84-110">値</span><span class="sxs-lookup"><span data-stu-id="e0a84-110">Value</span></span>|<span data-ttu-id="e0a84-111">説明</span><span class="sxs-lookup"><span data-stu-id="e0a84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0a84-112">noProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="e0a84-112">noProtectedAccessCredential</span></span>|<span data-ttu-id="e0a84-113">0</span><span class="sxs-lookup"><span data-stu-id="e0a84-113">0</span></span>|<span data-ttu-id="e0a84-114">EAP-FAST クリデンシャル (PAC) の保護されたアクセスなしを使用します。</span><span class="sxs-lookup"><span data-stu-id="e0a84-114">Use EAP-FAST without Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="e0a84-115">useProtectedAccessCredential</span><span class="sxs-lookup"><span data-stu-id="e0a84-115">useProtectedAccessCredential</span></span>|<span data-ttu-id="e0a84-116">1</span><span class="sxs-lookup"><span data-stu-id="e0a84-116">1</span></span>|<span data-ttu-id="e0a84-117">保護されたアクセス クリデンシャル (PAC) をを利用します。</span><span class="sxs-lookup"><span data-stu-id="e0a84-117">Use Protected Access Credential (PAC).</span></span>|
|<span data-ttu-id="e0a84-118">useProtectedAccessCredentialAndProvision</span><span class="sxs-lookup"><span data-stu-id="e0a84-118">useProtectedAccessCredentialAndProvision</span></span>|<span data-ttu-id="e0a84-119">2</span><span class="sxs-lookup"><span data-stu-id="e0a84-119">2</span></span>|<span data-ttu-id="e0a84-120">使用してアクセスを保護するクリデンシャル (PAC) と PAC. を提供します。</span><span class="sxs-lookup"><span data-stu-id="e0a84-120">Use Protected Access Credential (PAC) and Provision PAC.</span></span>|
|<span data-ttu-id="e0a84-121">useProtectedAccessCredentialAndProvisionAnonymously</span><span class="sxs-lookup"><span data-stu-id="e0a84-121">useProtectedAccessCredentialAndProvisionAnonymously</span></span>|<span data-ttu-id="e0a84-122">3</span><span class="sxs-lookup"><span data-stu-id="e0a84-122">3</span></span>|<span data-ttu-id="e0a84-123">保護されたアクセスの資格情報 (PAC)、PAC のプロビジョニングを使用して実行し、匿名で。</span><span class="sxs-lookup"><span data-stu-id="e0a84-123">Use Protected Access Credential (PAC), Provision PAC, and do so anonymously.</span></span>|




