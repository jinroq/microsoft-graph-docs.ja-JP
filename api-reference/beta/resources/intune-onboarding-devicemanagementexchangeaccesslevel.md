---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセスレベル。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 853cda5253f01b9d6b108d59de89bcc678def581
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940394"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="10086-103">deviceManagementExchangeAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="10086-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="10086-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10086-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10086-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="10086-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10086-106">Exchange のアクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="10086-106">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="10086-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="10086-107">Members</span></span>
|<span data-ttu-id="10086-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="10086-108">Member</span></span>|<span data-ttu-id="10086-109">値</span><span class="sxs-lookup"><span data-stu-id="10086-109">Value</span></span>|<span data-ttu-id="10086-110">説明</span><span class="sxs-lookup"><span data-stu-id="10086-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10086-111">none</span><span class="sxs-lookup"><span data-stu-id="10086-111">none</span></span>|<span data-ttu-id="10086-112">.0</span><span class="sxs-lookup"><span data-stu-id="10086-112">0</span></span>|<span data-ttu-id="10086-113">Exchange でデバイスアクセスルールが構成されていません。</span><span class="sxs-lookup"><span data-stu-id="10086-113">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="10086-114">使う</span><span class="sxs-lookup"><span data-stu-id="10086-114">allow</span></span>|<span data-ttu-id="10086-115">1-d</span><span class="sxs-lookup"><span data-stu-id="10086-115">1</span></span>|<span data-ttu-id="10086-116">デバイスへのアクセスを Exchange に許可します。</span><span class="sxs-lookup"><span data-stu-id="10086-116">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="10086-117">拒否</span><span class="sxs-lookup"><span data-stu-id="10086-117">block</span></span>|<span data-ttu-id="10086-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="10086-118">2</span></span>|<span data-ttu-id="10086-119">デバイスによる Exchange へのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="10086-119">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="10086-120">済み</span><span class="sxs-lookup"><span data-stu-id="10086-120">quarantine</span></span>|<span data-ttu-id="10086-121">1/3</span><span class="sxs-lookup"><span data-stu-id="10086-121">3</span></span>|<span data-ttu-id="10086-122">Exchange でデバイスを検疫します。</span><span class="sxs-lookup"><span data-stu-id="10086-122">Quarantine the device in Exchange.</span></span>|




