---
title: deviceManagementExchangeAccessLevel 列挙型
description: Exchange のアクセス レベルです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d24aedcd5c09de6e56b3870f8c5b111fbb39513
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414334"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="2961b-103">deviceManagementExchangeAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="2961b-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="2961b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2961b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2961b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2961b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2961b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2961b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2961b-107">Exchange のアクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="2961b-107">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="2961b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2961b-108">Members</span></span>
|<span data-ttu-id="2961b-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="2961b-109">Member</span></span>|<span data-ttu-id="2961b-110">値</span><span class="sxs-lookup"><span data-stu-id="2961b-110">Value</span></span>|<span data-ttu-id="2961b-111">説明</span><span class="sxs-lookup"><span data-stu-id="2961b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2961b-112">none</span><span class="sxs-lookup"><span data-stu-id="2961b-112">none</span></span>|<span data-ttu-id="2961b-113">0</span><span class="sxs-lookup"><span data-stu-id="2961b-113">0</span></span>|<span data-ttu-id="2961b-114">Exchange では、デバイス アクセス ルールが構成されていません。</span><span class="sxs-lookup"><span data-stu-id="2961b-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="2961b-115">許可します。</span><span class="sxs-lookup"><span data-stu-id="2961b-115">allow</span></span>|<span data-ttu-id="2961b-116">1</span><span class="sxs-lookup"><span data-stu-id="2961b-116">1</span></span>|<span data-ttu-id="2961b-117">デバイスの Exchange へのアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="2961b-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="2961b-118">ブロック</span><span class="sxs-lookup"><span data-stu-id="2961b-118">block</span></span>|<span data-ttu-id="2961b-119">2</span><span class="sxs-lookup"><span data-stu-id="2961b-119">2</span></span>|<span data-ttu-id="2961b-120">デバイスから Exchange へのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2961b-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="2961b-121">検査</span><span class="sxs-lookup"><span data-stu-id="2961b-121">quarantine</span></span>|<span data-ttu-id="2961b-122">3</span><span class="sxs-lookup"><span data-stu-id="2961b-122">3</span></span>|<span data-ttu-id="2961b-123">デバイスを Exchange で隔離します。</span><span class="sxs-lookup"><span data-stu-id="2961b-123">Quarantine the device in Exchange.</span></span>|




