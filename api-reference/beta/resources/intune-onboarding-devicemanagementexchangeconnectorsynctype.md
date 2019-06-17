---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04cd9e55b03e21bd4e99c56144ea05cabd1ecd7b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993005"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="19ad4-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="19ad4-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="19ad4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19ad4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19ad4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="19ad4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19ad4-106">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="19ad4-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="19ad4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="19ad4-107">Members</span></span>
|<span data-ttu-id="19ad4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="19ad4-108">Member</span></span>|<span data-ttu-id="19ad4-109">値</span><span class="sxs-lookup"><span data-stu-id="19ad4-109">Value</span></span>|<span data-ttu-id="19ad4-110">説明</span><span class="sxs-lookup"><span data-stu-id="19ad4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19ad4-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="19ad4-111">fullSync</span></span>|<span data-ttu-id="19ad4-112">.0</span><span class="sxs-lookup"><span data-stu-id="19ad4-112">0</span></span>|<span data-ttu-id="19ad4-113">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="19ad4-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="19ad4-114">Deltasync]</span><span class="sxs-lookup"><span data-stu-id="19ad4-114">deltaSync</span></span>|<span data-ttu-id="19ad4-115">1-d</span><span class="sxs-lookup"><span data-stu-id="19ad4-115">1</span></span>|<span data-ttu-id="19ad4-116">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="19ad4-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





