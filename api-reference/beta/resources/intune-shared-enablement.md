---
title: 列挙型の有効化
description: '値は、デバイスの状態を示すために使用します。 '
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c77da7026640e9ad0a6f6f08f077d509cb411f22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888257"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="6d07e-103">列挙型の有効化</span><span class="sxs-lookup"><span data-stu-id="6d07e-103">enablement enum type</span></span>

> <span data-ttu-id="6d07e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6d07e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d07e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d07e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6d07e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d07e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d07e-107">値は、デバイスの状態を示すために使用します。</span><span class="sxs-lookup"><span data-stu-id="6d07e-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="6d07e-108">間に違いがあることに注意が無効になり、構成されていません。</span><span class="sxs-lookup"><span data-stu-id="6d07e-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="6d07e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6d07e-109">Members</span></span>
|<span data-ttu-id="6d07e-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="6d07e-110">Member</span></span>|<span data-ttu-id="6d07e-111">値</span><span class="sxs-lookup"><span data-stu-id="6d07e-111">Value</span></span>|<span data-ttu-id="6d07e-112">説明</span><span class="sxs-lookup"><span data-stu-id="6d07e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d07e-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6d07e-113">notConfigured</span></span>|<span data-ttu-id="6d07e-114">0</span><span class="sxs-lookup"><span data-stu-id="6d07e-114">0</span></span>|<span data-ttu-id="6d07e-115">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="6d07e-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="6d07e-116">enabled</span><span class="sxs-lookup"><span data-stu-id="6d07e-116">enabled</span></span>|<span data-ttu-id="6d07e-117">1</span><span class="sxs-lookup"><span data-stu-id="6d07e-117">1</span></span>|<span data-ttu-id="6d07e-118">デバイスの設定を有効にします。</span><span class="sxs-lookup"><span data-stu-id="6d07e-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="6d07e-119">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="6d07e-119">disabled</span></span>|<span data-ttu-id="6d07e-120">2</span><span class="sxs-lookup"><span data-stu-id="6d07e-120">2</span></span>|<span data-ttu-id="6d07e-121">デバイスの設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="6d07e-121">Disables the setting on the device.</span></span>|
