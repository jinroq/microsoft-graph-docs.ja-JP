---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22622c993017539e97e9a8913267eb4fe0205c5d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940324"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="a92cf-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a92cf-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="a92cf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a92cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a92cf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a92cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a92cf-106">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="a92cf-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="a92cf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a92cf-107">Members</span></span>
|<span data-ttu-id="a92cf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a92cf-108">Member</span></span>|<span data-ttu-id="a92cf-109">値</span><span class="sxs-lookup"><span data-stu-id="a92cf-109">Value</span></span>|<span data-ttu-id="a92cf-110">説明</span><span class="sxs-lookup"><span data-stu-id="a92cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a92cf-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="a92cf-111">fullSync</span></span>|<span data-ttu-id="a92cf-112">.0</span><span class="sxs-lookup"><span data-stu-id="a92cf-112">0</span></span>|<span data-ttu-id="a92cf-113">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="a92cf-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="a92cf-114">Deltasync]</span><span class="sxs-lookup"><span data-stu-id="a92cf-114">deltaSync</span></span>|<span data-ttu-id="a92cf-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a92cf-115">1</span></span>|<span data-ttu-id="a92cf-116">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="a92cf-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




