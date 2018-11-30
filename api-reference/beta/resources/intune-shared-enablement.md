---
title: 列挙型の有効化
description: '値は、デバイスの状態を示すために使用します。 '
ms.openlocfilehash: 5e72df98d33a7d3502dae4bc369781b69bc6aeb0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070103"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="70077-103">列挙型の有効化</span><span class="sxs-lookup"><span data-stu-id="70077-103">enablement enum type</span></span>

> <span data-ttu-id="70077-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="70077-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70077-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70077-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70077-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="70077-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70077-107">値は、デバイスの状態を示すために使用します。</span><span class="sxs-lookup"><span data-stu-id="70077-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="70077-108">間に違いがあることに注意が無効になり、構成されていません。</span><span class="sxs-lookup"><span data-stu-id="70077-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="70077-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="70077-109">Members</span></span>
|<span data-ttu-id="70077-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="70077-110">Member</span></span>|<span data-ttu-id="70077-111">値</span><span class="sxs-lookup"><span data-stu-id="70077-111">Value</span></span>|<span data-ttu-id="70077-112">説明</span><span class="sxs-lookup"><span data-stu-id="70077-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70077-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="70077-113">notConfigured</span></span>|<span data-ttu-id="70077-114">0</span><span class="sxs-lookup"><span data-stu-id="70077-114">0</span></span>|<span data-ttu-id="70077-115">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="70077-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="70077-116">enabled</span><span class="sxs-lookup"><span data-stu-id="70077-116">enabled</span></span>|<span data-ttu-id="70077-117">1</span><span class="sxs-lookup"><span data-stu-id="70077-117">1</span></span>|<span data-ttu-id="70077-118">デバイスの設定を有効にします。</span><span class="sxs-lookup"><span data-stu-id="70077-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="70077-119">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="70077-119">disabled</span></span>|<span data-ttu-id="70077-120">2</span><span class="sxs-lookup"><span data-stu-id="70077-120">2</span></span>|<span data-ttu-id="70077-121">デバイスの設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="70077-121">Disables the setting on the device.</span></span>|
