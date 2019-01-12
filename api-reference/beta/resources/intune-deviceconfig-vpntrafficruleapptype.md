---
title: vpnTrafficRuleAppType 列挙型
description: VPN トラフィックの規則が関連付けられているアプリケーションの種類を示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6adf30f981bcb3ee4d57410a63419b29ac4184cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937743"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="f4247-103">vpnTrafficRuleAppType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f4247-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="f4247-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f4247-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4247-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4247-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4247-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4247-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4247-107">VPN トラフィックの規則が関連付けられているアプリケーションの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="f4247-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>
## <a name="members"></a><span data-ttu-id="f4247-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f4247-108">Members</span></span>
|<span data-ttu-id="f4247-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f4247-109">Member</span></span>|<span data-ttu-id="f4247-110">値</span><span class="sxs-lookup"><span data-stu-id="f4247-110">Value</span></span>|<span data-ttu-id="f4247-111">説明</span><span class="sxs-lookup"><span data-stu-id="f4247-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4247-112">none</span><span class="sxs-lookup"><span data-stu-id="f4247-112">none</span></span>|<span data-ttu-id="f4247-113">0</span><span class="sxs-lookup"><span data-stu-id="f4247-113">0</span></span>|<span data-ttu-id="f4247-114">トラフィックの規則は、アプリケーションに関連付けられているではありません。</span><span class="sxs-lookup"><span data-stu-id="f4247-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="f4247-115">デスクトップ</span><span class="sxs-lookup"><span data-stu-id="f4247-115">desktop</span></span>|<span data-ttu-id="f4247-116">1</span><span class="sxs-lookup"><span data-stu-id="f4247-116">1</span></span>|<span data-ttu-id="f4247-117">トラフィックの規則では、デスクトップ アプリケーションに関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="f4247-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="f4247-118">ユニバーサル</span><span class="sxs-lookup"><span data-stu-id="f4247-118">universal</span></span>|<span data-ttu-id="f4247-119">2</span><span class="sxs-lookup"><span data-stu-id="f4247-119">2</span></span>|<span data-ttu-id="f4247-120">トラフィックの規則では、汎用のアプリケーションに関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="f4247-120">The traffic rule is associated with a Universal app.</span></span>|





