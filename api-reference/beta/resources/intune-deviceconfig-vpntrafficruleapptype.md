---
title: vpnTrafficRuleAppType 列挙型
description: VPN トラフィックルールが関連付けられているアプリの種類を示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1762e952bbebfc985f9af9694bfb14e0bdd7d19f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367548"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="ba362-103">vpnTrafficRuleAppType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ba362-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="ba362-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba362-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba362-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba362-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba362-106">VPN トラフィックルールが関連付けられているアプリの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ba362-106">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="ba362-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ba362-107">Members</span></span>
|<span data-ttu-id="ba362-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ba362-108">Member</span></span>|<span data-ttu-id="ba362-109">値</span><span class="sxs-lookup"><span data-stu-id="ba362-109">Value</span></span>|<span data-ttu-id="ba362-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba362-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba362-111">none</span><span class="sxs-lookup"><span data-stu-id="ba362-111">none</span></span>|<span data-ttu-id="ba362-112">.0</span><span class="sxs-lookup"><span data-stu-id="ba362-112">0</span></span>|<span data-ttu-id="ba362-113">トラフィックルールがアプリに関連付けられていません。</span><span class="sxs-lookup"><span data-stu-id="ba362-113">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="ba362-114">コンピューター</span><span class="sxs-lookup"><span data-stu-id="ba362-114">desktop</span></span>|<span data-ttu-id="ba362-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ba362-115">1</span></span>|<span data-ttu-id="ba362-116">トラフィックルールは、デスクトップアプリに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="ba362-116">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="ba362-117">ユニバーサル</span><span class="sxs-lookup"><span data-stu-id="ba362-117">universal</span></span>|<span data-ttu-id="ba362-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ba362-118">2</span></span>|<span data-ttu-id="ba362-119">トラフィックルールはユニバーサルアプリに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="ba362-119">The traffic rule is associated with a Universal app.</span></span>|



