---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
author: tfitzmac
ms.openlocfilehash: dcad9b1455d488c9243b57f607281b39857cbf25
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316850"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="d8c66-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d8c66-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="d8c66-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d8c66-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8c66-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8c66-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8c66-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8c66-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8c66-107">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="d8c66-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="d8c66-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d8c66-108">Members</span></span>
|<span data-ttu-id="d8c66-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d8c66-109">Member</span></span>|<span data-ttu-id="d8c66-110">値</span><span class="sxs-lookup"><span data-stu-id="d8c66-110">Value</span></span>|<span data-ttu-id="d8c66-111">説明</span><span class="sxs-lookup"><span data-stu-id="d8c66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8c66-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="d8c66-112">fullSync</span></span>|<span data-ttu-id="d8c66-113">0</span><span class="sxs-lookup"><span data-stu-id="d8c66-113">0</span></span>|<span data-ttu-id="d8c66-114">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="d8c66-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="d8c66-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="d8c66-115">deltaSync</span></span>|<span data-ttu-id="d8c66-116">1</span><span class="sxs-lookup"><span data-stu-id="d8c66-116">1</span></span>|<span data-ttu-id="d8c66-117">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="d8c66-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





