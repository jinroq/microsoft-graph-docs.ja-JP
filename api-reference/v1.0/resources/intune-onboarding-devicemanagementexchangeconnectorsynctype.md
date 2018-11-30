---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
ms.openlocfilehash: 123a1071db74e931cd80d8d735c83af8a7ef86f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022269"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="c2a74-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c2a74-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="c2a74-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2a74-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2a74-105">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="c2a74-105">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="c2a74-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="c2a74-106">Members</span></span>
|<span data-ttu-id="c2a74-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c2a74-107">Member</span></span>|<span data-ttu-id="c2a74-108">値</span><span class="sxs-lookup"><span data-stu-id="c2a74-108">Value</span></span>|<span data-ttu-id="c2a74-109">説明</span><span class="sxs-lookup"><span data-stu-id="c2a74-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2a74-110">fullSync</span><span class="sxs-lookup"><span data-stu-id="c2a74-110">fullSync</span></span>|<span data-ttu-id="c2a74-111">0</span><span class="sxs-lookup"><span data-stu-id="c2a74-111">0</span></span>|<span data-ttu-id="c2a74-112">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="c2a74-112">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="c2a74-113">deltaSync</span><span class="sxs-lookup"><span data-stu-id="c2a74-113">deltaSync</span></span>|<span data-ttu-id="c2a74-114">1</span><span class="sxs-lookup"><span data-stu-id="c2a74-114">1</span></span>|<span data-ttu-id="c2a74-115">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="c2a74-115">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|



