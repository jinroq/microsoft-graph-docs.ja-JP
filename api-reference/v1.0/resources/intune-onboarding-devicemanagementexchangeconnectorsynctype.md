---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdd1da2ecec6fb7848787386991ee09741d0b67
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257583"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="aa243-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="aa243-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="aa243-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa243-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa243-105">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="aa243-105">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="aa243-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="aa243-106">Members</span></span>
|<span data-ttu-id="aa243-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="aa243-107">Member</span></span>|<span data-ttu-id="aa243-108">値</span><span class="sxs-lookup"><span data-stu-id="aa243-108">Value</span></span>|<span data-ttu-id="aa243-109">説明</span><span class="sxs-lookup"><span data-stu-id="aa243-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa243-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="aa243-110">fullSync</span></span>|<span data-ttu-id="aa243-111">.0</span><span class="sxs-lookup"><span data-stu-id="aa243-111">0</span></span>|<span data-ttu-id="aa243-112">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="aa243-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="aa243-113">deltasync]</span><span class="sxs-lookup"><span data-stu-id="aa243-113">deltaSync</span></span>|<span data-ttu-id="aa243-114">1-d</span><span class="sxs-lookup"><span data-stu-id="aa243-114">1</span></span>|<span data-ttu-id="aa243-115">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="aa243-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



