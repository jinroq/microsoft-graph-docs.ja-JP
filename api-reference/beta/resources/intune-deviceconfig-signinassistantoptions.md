---
title: signInAssistantOptions 列挙型
description: 値は、SignInAssistantSettings です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f80b67a40d0b551386b9f03273efb26e294d3520
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825397"
---
# <a name="signinassistantoptions-enum-type"></a><span data-ttu-id="2c9df-103">signInAssistantOptions 列挙型</span><span class="sxs-lookup"><span data-stu-id="2c9df-103">signInAssistantOptions enum type</span></span>

> <span data-ttu-id="2c9df-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2c9df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c9df-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c9df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c9df-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c9df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c9df-107">値は、SignInAssistantSettings です。</span><span class="sxs-lookup"><span data-stu-id="2c9df-107">Values for the SignInAssistantSettings.</span></span>
## <a name="members"></a><span data-ttu-id="2c9df-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2c9df-108">Members</span></span>
|<span data-ttu-id="2c9df-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="2c9df-109">Member</span></span>|<span data-ttu-id="2c9df-110">値</span><span class="sxs-lookup"><span data-stu-id="2c9df-110">Value</span></span>|<span data-ttu-id="2c9df-111">説明</span><span class="sxs-lookup"><span data-stu-id="2c9df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c9df-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2c9df-112">notConfigured</span></span>|<span data-ttu-id="2c9df-113">0</span><span class="sxs-lookup"><span data-stu-id="2c9df-113">0</span></span>|<span data-ttu-id="2c9df-114">構成されていません - wlidsvc の開始は、SERVICE_DEMAND_START に設定されます。</span><span class="sxs-lookup"><span data-stu-id="2c9df-114">Not configured - wlidsvc Start will be set to SERVICE_DEMAND_START.</span></span>|
|<span data-ttu-id="2c9df-115">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="2c9df-115">disabled</span></span>|<span data-ttu-id="2c9df-116">1</span><span class="sxs-lookup"><span data-stu-id="2c9df-116">1</span></span>|<span data-ttu-id="2c9df-117">無効 - wlidsvc 開始を SERVICE_DISABLED に設定されます。</span><span class="sxs-lookup"><span data-stu-id="2c9df-117">Disabled - wlidsvc Start will be set to SERVICE_DISABLED.</span></span>|





