---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 33262ce8eb53b03af17a409d6fa5cd3e1dcd3357
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870582"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="48920-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="48920-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="48920-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="48920-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48920-105">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="48920-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="48920-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="48920-106">Members</span></span>
|<span data-ttu-id="48920-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="48920-107">Member</span></span>|<span data-ttu-id="48920-108">値</span><span class="sxs-lookup"><span data-stu-id="48920-108">Value</span></span>|<span data-ttu-id="48920-109">説明</span><span class="sxs-lookup"><span data-stu-id="48920-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48920-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="48920-110">fullSync</span></span>|<span data-ttu-id="48920-111">0</span><span class="sxs-lookup"><span data-stu-id="48920-111">0</span></span>|<span data-ttu-id="48920-112">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="48920-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="48920-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="48920-113">deltaSync</span></span>|<span data-ttu-id="48920-114">1</span><span class="sxs-lookup"><span data-stu-id="48920-114">1</span></span>|<span data-ttu-id="48920-115">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="48920-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



