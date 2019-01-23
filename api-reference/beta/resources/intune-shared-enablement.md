---
title: 列挙型の有効化
description: Intune は、複数のワークフローをサポートするため Microsoft グラフ API の対応の列挙体について説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 538b52790cf7748453adfda2a6bea8334a36fb87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399564"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="37489-103">列挙型の有効化</span><span class="sxs-lookup"><span data-stu-id="37489-103">enablement enum type</span></span>

> <span data-ttu-id="37489-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="37489-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37489-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37489-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37489-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="37489-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37489-107">値は、デバイスの状態を示すために使用します。</span><span class="sxs-lookup"><span data-stu-id="37489-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="37489-108">間に違いがあることに注意が無効になり、構成されていません。</span><span class="sxs-lookup"><span data-stu-id="37489-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="37489-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="37489-109">Members</span></span>
|<span data-ttu-id="37489-110">メンバー</span><span class="sxs-lookup"><span data-stu-id="37489-110">Member</span></span>|<span data-ttu-id="37489-111">値</span><span class="sxs-lookup"><span data-stu-id="37489-111">Value</span></span>|<span data-ttu-id="37489-112">説明</span><span class="sxs-lookup"><span data-stu-id="37489-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37489-113">notConfigured</span><span class="sxs-lookup"><span data-stu-id="37489-113">notConfigured</span></span>|<span data-ttu-id="37489-114">0</span><span class="sxs-lookup"><span data-stu-id="37489-114">0</span></span>|<span data-ttu-id="37489-115">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="37489-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="37489-116">enabled</span><span class="sxs-lookup"><span data-stu-id="37489-116">enabled</span></span>|<span data-ttu-id="37489-117">1</span><span class="sxs-lookup"><span data-stu-id="37489-117">1</span></span>|<span data-ttu-id="37489-118">デバイスの設定を有効にします。</span><span class="sxs-lookup"><span data-stu-id="37489-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="37489-119">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="37489-119">disabled</span></span>|<span data-ttu-id="37489-120">2</span><span class="sxs-lookup"><span data-stu-id="37489-120">2</span></span>|<span data-ttu-id="37489-121">デバイスの設定を無効にします。</span><span class="sxs-lookup"><span data-stu-id="37489-121">Disables the setting on the device.</span></span>|
