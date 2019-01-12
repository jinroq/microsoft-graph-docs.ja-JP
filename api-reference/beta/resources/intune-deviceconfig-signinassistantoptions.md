---
title: signInAssistantOptions 列挙型
description: 値は、SignInAssistantSettings です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ef8bd0252c429d5fe9ee8b0c02a07651140eb45d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934682"
---
# <a name="signinassistantoptions-enum-type"></a><span data-ttu-id="04ffe-103">signInAssistantOptions 列挙型</span><span class="sxs-lookup"><span data-stu-id="04ffe-103">signInAssistantOptions enum type</span></span>

> <span data-ttu-id="04ffe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04ffe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04ffe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04ffe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04ffe-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04ffe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04ffe-107">値は、SignInAssistantSettings です。</span><span class="sxs-lookup"><span data-stu-id="04ffe-107">Values for the SignInAssistantSettings.</span></span>
## <a name="members"></a><span data-ttu-id="04ffe-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="04ffe-108">Members</span></span>
|<span data-ttu-id="04ffe-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="04ffe-109">Member</span></span>|<span data-ttu-id="04ffe-110">値</span><span class="sxs-lookup"><span data-stu-id="04ffe-110">Value</span></span>|<span data-ttu-id="04ffe-111">説明</span><span class="sxs-lookup"><span data-stu-id="04ffe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04ffe-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="04ffe-112">notConfigured</span></span>|<span data-ttu-id="04ffe-113">0</span><span class="sxs-lookup"><span data-stu-id="04ffe-113">0</span></span>|<span data-ttu-id="04ffe-114">構成されていません - wlidsvc の開始は、SERVICE_DEMAND_START に設定されます。</span><span class="sxs-lookup"><span data-stu-id="04ffe-114">Not configured - wlidsvc Start will be set to SERVICE_DEMAND_START.</span></span>|
|<span data-ttu-id="04ffe-115">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="04ffe-115">disabled</span></span>|<span data-ttu-id="04ffe-116">1</span><span class="sxs-lookup"><span data-stu-id="04ffe-116">1</span></span>|<span data-ttu-id="04ffe-117">無効 - wlidsvc 開始を SERVICE_DISABLED に設定されます。</span><span class="sxs-lookup"><span data-stu-id="04ffe-117">Disabled - wlidsvc Start will be set to SERVICE_DISABLED.</span></span>|





