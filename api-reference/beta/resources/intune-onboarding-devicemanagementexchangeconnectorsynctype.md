---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bc62e03f61a5170b5495300b0c7f5182262ddafb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851773"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="fe0c6-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="fe0c6-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="fe0c6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe0c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe0c6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe0c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe0c6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe0c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe0c6-107">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="fe0c6-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="fe0c6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fe0c6-108">Members</span></span>
|<span data-ttu-id="fe0c6-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="fe0c6-109">Member</span></span>|<span data-ttu-id="fe0c6-110">値</span><span class="sxs-lookup"><span data-stu-id="fe0c6-110">Value</span></span>|<span data-ttu-id="fe0c6-111">説明</span><span class="sxs-lookup"><span data-stu-id="fe0c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe0c6-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="fe0c6-112">fullSync</span></span>|<span data-ttu-id="fe0c6-113">0</span><span class="sxs-lookup"><span data-stu-id="fe0c6-113">0</span></span>|<span data-ttu-id="fe0c6-114">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="fe0c6-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="fe0c6-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="fe0c6-115">deltaSync</span></span>|<span data-ttu-id="fe0c6-116">1</span><span class="sxs-lookup"><span data-stu-id="fe0c6-116">1</span></span>|<span data-ttu-id="fe0c6-117">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="fe0c6-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





