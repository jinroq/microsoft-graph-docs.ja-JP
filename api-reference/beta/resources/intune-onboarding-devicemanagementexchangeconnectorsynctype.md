---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac6f54c2a09752df2382ae6b27f9dc9387262acf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912730"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="f07d3-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f07d3-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="f07d3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f07d3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f07d3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f07d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f07d3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f07d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f07d3-107">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="f07d3-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="f07d3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f07d3-108">Members</span></span>
|<span data-ttu-id="f07d3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="f07d3-109">Member</span></span>|<span data-ttu-id="f07d3-110">値</span><span class="sxs-lookup"><span data-stu-id="f07d3-110">Value</span></span>|<span data-ttu-id="f07d3-111">説明</span><span class="sxs-lookup"><span data-stu-id="f07d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f07d3-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="f07d3-112">fullSync</span></span>|<span data-ttu-id="f07d3-113">0</span><span class="sxs-lookup"><span data-stu-id="f07d3-113">0</span></span>|<span data-ttu-id="f07d3-114">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="f07d3-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="f07d3-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="f07d3-115">deltaSync</span></span>|<span data-ttu-id="f07d3-116">1</span><span class="sxs-lookup"><span data-stu-id="f07d3-116">1</span></span>|<span data-ttu-id="f07d3-117">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="f07d3-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





