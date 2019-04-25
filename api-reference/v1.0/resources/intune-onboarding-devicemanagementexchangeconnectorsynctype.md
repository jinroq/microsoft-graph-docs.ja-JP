---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdd1da2ecec6fb7848787386991ee09741d0b67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565931"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="91d2b-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="91d2b-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="91d2b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91d2b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91d2b-105">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="91d2b-105">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="91d2b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="91d2b-106">Members</span></span>
|<span data-ttu-id="91d2b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="91d2b-107">Member</span></span>|<span data-ttu-id="91d2b-108">値</span><span class="sxs-lookup"><span data-stu-id="91d2b-108">Value</span></span>|<span data-ttu-id="91d2b-109">説明</span><span class="sxs-lookup"><span data-stu-id="91d2b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91d2b-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="91d2b-110">fullSync</span></span>|<span data-ttu-id="91d2b-111">.0</span><span class="sxs-lookup"><span data-stu-id="91d2b-111">0</span></span>|<span data-ttu-id="91d2b-112">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="91d2b-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="91d2b-113">deltasync]</span><span class="sxs-lookup"><span data-stu-id="91d2b-113">deltaSync</span></span>|<span data-ttu-id="91d2b-114">1 </span><span class="sxs-lookup"><span data-stu-id="91d2b-114">1</span></span>|<span data-ttu-id="91d2b-115">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="91d2b-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



