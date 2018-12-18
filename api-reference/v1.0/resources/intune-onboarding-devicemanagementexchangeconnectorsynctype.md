---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
author: tfitzmac
ms.openlocfilehash: 1915de3305cb8e41609dd2101f246a8e003f60f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312076"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="5d16c-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5d16c-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="5d16c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5d16c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d16c-105">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="5d16c-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="5d16c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="5d16c-106">Members</span></span>
|<span data-ttu-id="5d16c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5d16c-107">Member</span></span>|<span data-ttu-id="5d16c-108">値</span><span class="sxs-lookup"><span data-stu-id="5d16c-108">Value</span></span>|<span data-ttu-id="5d16c-109">説明</span><span class="sxs-lookup"><span data-stu-id="5d16c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d16c-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="5d16c-110">fullSync</span></span>|<span data-ttu-id="5d16c-111">0</span><span class="sxs-lookup"><span data-stu-id="5d16c-111">0</span></span>|<span data-ttu-id="5d16c-112">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="5d16c-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="5d16c-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="5d16c-113">deltaSync</span></span>|<span data-ttu-id="5d16c-114">1</span><span class="sxs-lookup"><span data-stu-id="5d16c-114">1</span></span>|<span data-ttu-id="5d16c-115">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="5d16c-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



