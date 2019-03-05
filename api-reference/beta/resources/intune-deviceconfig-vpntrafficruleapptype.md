---
title: vpnTrafficRuleAppType 列挙型
description: VPN トラフィックルールが関連付けられているアプリの種類を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb8be06a43c64dcb766da479414fcc437ee49cb9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140531"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="356c1-103">vpnTrafficRuleAppType 列挙型</span><span class="sxs-lookup"><span data-stu-id="356c1-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="356c1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="356c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="356c1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="356c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="356c1-106">VPN トラフィックルールが関連付けられているアプリの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="356c1-106">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="356c1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="356c1-107">Members</span></span>
|<span data-ttu-id="356c1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="356c1-108">Member</span></span>|<span data-ttu-id="356c1-109">値</span><span class="sxs-lookup"><span data-stu-id="356c1-109">Value</span></span>|<span data-ttu-id="356c1-110">説明</span><span class="sxs-lookup"><span data-stu-id="356c1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="356c1-111">none</span><span class="sxs-lookup"><span data-stu-id="356c1-111">none</span></span>|<span data-ttu-id="356c1-112">.0</span><span class="sxs-lookup"><span data-stu-id="356c1-112">0</span></span>|<span data-ttu-id="356c1-113">トラフィックルールがアプリに関連付けられていません。</span><span class="sxs-lookup"><span data-stu-id="356c1-113">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="356c1-114">コンピューター</span><span class="sxs-lookup"><span data-stu-id="356c1-114">desktop</span></span>|<span data-ttu-id="356c1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="356c1-115">1</span></span>|<span data-ttu-id="356c1-116">トラフィックルールは、デスクトップアプリに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="356c1-116">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="356c1-117">ユニバーサル</span><span class="sxs-lookup"><span data-stu-id="356c1-117">universal</span></span>|<span data-ttu-id="356c1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="356c1-118">2</span></span>|<span data-ttu-id="356c1-119">トラフィックルールはユニバーサルアプリに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="356c1-119">The traffic rule is associated with a Universal app.</span></span>|




