---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: 要求された Exchange Connector の同期の種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 86cdc6277232985d4c3e247c5c14801a5d3aef54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010764"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="45608-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="45608-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="45608-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45608-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45608-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45608-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45608-106">要求された Exchange Connector の同期の種類。</span><span class="sxs-lookup"><span data-stu-id="45608-106">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="45608-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="45608-107">Members</span></span>
|<span data-ttu-id="45608-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="45608-108">Member</span></span>|<span data-ttu-id="45608-109">値</span><span class="sxs-lookup"><span data-stu-id="45608-109">Value</span></span>|<span data-ttu-id="45608-110">説明</span><span class="sxs-lookup"><span data-stu-id="45608-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45608-111">fullSync</span><span class="sxs-lookup"><span data-stu-id="45608-111">fullSync</span></span>|<span data-ttu-id="45608-112">.0</span><span class="sxs-lookup"><span data-stu-id="45608-112">0</span></span>|<span data-ttu-id="45608-113">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="45608-113">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="45608-114">Deltasync]</span><span class="sxs-lookup"><span data-stu-id="45608-114">deltaSync</span></span>|<span data-ttu-id="45608-115">1-d</span><span class="sxs-lookup"><span data-stu-id="45608-115">1</span></span>|<span data-ttu-id="45608-116">[差分同期] ウィンドウで更新された Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="45608-116">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





