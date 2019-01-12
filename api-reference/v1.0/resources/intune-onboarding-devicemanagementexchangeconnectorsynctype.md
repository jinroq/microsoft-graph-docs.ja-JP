---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5af14006bd6f3cc8733faecc8e0219cc02e7fcd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983283"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="50a78-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="50a78-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="50a78-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="50a78-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50a78-105">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="50a78-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="50a78-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="50a78-106">Members</span></span>
|<span data-ttu-id="50a78-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="50a78-107">Member</span></span>|<span data-ttu-id="50a78-108">値</span><span class="sxs-lookup"><span data-stu-id="50a78-108">Value</span></span>|<span data-ttu-id="50a78-109">説明</span><span class="sxs-lookup"><span data-stu-id="50a78-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50a78-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="50a78-110">fullSync</span></span>|<span data-ttu-id="50a78-111">0</span><span class="sxs-lookup"><span data-stu-id="50a78-111">0</span></span>|<span data-ttu-id="50a78-112">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="50a78-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="50a78-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="50a78-113">deltaSync</span></span>|<span data-ttu-id="50a78-114">1</span><span class="sxs-lookup"><span data-stu-id="50a78-114">1</span></span>|<span data-ttu-id="50a78-115">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="50a78-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



