---
title: 列挙型の有効化
description: '値は、デバイスの状態を示すために使用します。 '
author: tfitzmac
ms.openlocfilehash: 5b1d494fd116eab437b4654d396b029e1384a817
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356890"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="1c316-103">列挙型の有効化</span><span class="sxs-lookup"><span data-stu-id="1c316-103">enablement enum type</span></span>

> <span data-ttu-id="1c316-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1c316-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c316-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c316-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1c316-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c316-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c316-107">値は、デバイスの状態を示すために使用します。</span><span class="sxs-lookup"><span data-stu-id="1c316-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="1c316-108">間に違いがあることに注意が無効になり、構成されていません。</span><span class="sxs-lookup"><span data-stu-id="1c316-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="1c316-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1c316-109">Members</span></span>
|<span data-ttu-id="1c316-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="1c316-110">Member</span></span>|<span data-ttu-id="1c316-111">値</span><span class="sxs-lookup"><span data-stu-id="1c316-111">Value</span></span>|<span data-ttu-id="1c316-112">説明</span><span class="sxs-lookup"><span data-stu-id="1c316-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c316-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1c316-113">notConfigured</span></span>|<span data-ttu-id="1c316-114">0</span><span class="sxs-lookup"><span data-stu-id="1c316-114">0</span></span>|<span data-ttu-id="1c316-115">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="1c316-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="1c316-116">enabled</span><span class="sxs-lookup"><span data-stu-id="1c316-116">enabled</span></span>|<span data-ttu-id="1c316-117">1</span><span class="sxs-lookup"><span data-stu-id="1c316-117">1</span></span>|<span data-ttu-id="1c316-118">デバイスの設定を有効にします。</span><span class="sxs-lookup"><span data-stu-id="1c316-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="1c316-119">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="1c316-119">disabled</span></span>|<span data-ttu-id="1c316-120">2</span><span class="sxs-lookup"><span data-stu-id="1c316-120">2</span></span>|<span data-ttu-id="1c316-121">デバイスの設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="1c316-121">Disables the setting on the device.</span></span>|
