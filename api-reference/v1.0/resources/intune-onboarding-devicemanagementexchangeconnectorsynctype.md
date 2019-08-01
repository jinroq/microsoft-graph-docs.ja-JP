---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0066b6b4fce924df8c5101228db8868da7e1b743
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037444"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="6f866-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6f866-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="6f866-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f866-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f866-105">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="6f866-105">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="6f866-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="6f866-106">Members</span></span>
|<span data-ttu-id="6f866-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6f866-107">Member</span></span>|<span data-ttu-id="6f866-108">値</span><span class="sxs-lookup"><span data-stu-id="6f866-108">Value</span></span>|<span data-ttu-id="6f866-109">説明</span><span class="sxs-lookup"><span data-stu-id="6f866-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f866-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="6f866-110">fullSync</span></span>|<span data-ttu-id="6f866-111">.0</span><span class="sxs-lookup"><span data-stu-id="6f866-111">0</span></span>|<span data-ttu-id="6f866-112">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="6f866-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="6f866-113">Deltasync]</span><span class="sxs-lookup"><span data-stu-id="6f866-113">deltaSync</span></span>|<span data-ttu-id="6f866-114">1-d</span><span class="sxs-lookup"><span data-stu-id="6f866-114">1</span></span>|<span data-ttu-id="6f866-115">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="6f866-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



