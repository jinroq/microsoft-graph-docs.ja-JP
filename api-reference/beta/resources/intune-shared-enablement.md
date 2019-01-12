---
title: 列挙型の有効化
description: '値は、デバイスの状態を示すために使用します。 '
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 539d57111003f348147a6be3952d969ab4206b5d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911960"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="a5963-103">列挙型の有効化</span><span class="sxs-lookup"><span data-stu-id="a5963-103">enablement enum type</span></span>

> <span data-ttu-id="a5963-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5963-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5963-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5963-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5963-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5963-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5963-107">値は、デバイスの状態を示すために使用します。</span><span class="sxs-lookup"><span data-stu-id="a5963-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="a5963-108">間に違いがあることに注意が無効になり、構成されていません。</span><span class="sxs-lookup"><span data-stu-id="a5963-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="a5963-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a5963-109">Members</span></span>
|<span data-ttu-id="a5963-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="a5963-110">Member</span></span>|<span data-ttu-id="a5963-111">値</span><span class="sxs-lookup"><span data-stu-id="a5963-111">Value</span></span>|<span data-ttu-id="a5963-112">説明</span><span class="sxs-lookup"><span data-stu-id="a5963-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5963-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a5963-113">notConfigured</span></span>|<span data-ttu-id="a5963-114">0</span><span class="sxs-lookup"><span data-stu-id="a5963-114">0</span></span>|<span data-ttu-id="a5963-115">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="a5963-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="a5963-116">enabled</span><span class="sxs-lookup"><span data-stu-id="a5963-116">enabled</span></span>|<span data-ttu-id="a5963-117">1</span><span class="sxs-lookup"><span data-stu-id="a5963-117">1</span></span>|<span data-ttu-id="a5963-118">デバイスの設定を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a5963-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="a5963-119">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="a5963-119">disabled</span></span>|<span data-ttu-id="a5963-120">2</span><span class="sxs-lookup"><span data-stu-id="a5963-120">2</span></span>|<span data-ttu-id="a5963-121">デバイスの設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="a5963-121">Disables the setting on the device.</span></span>|
