---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange コネクタの現在の状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 455d7ecbe2d22de7825faf36e743f830480a5737
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928278"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="a8a0f-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="a8a0f-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="a8a0f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8a0f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8a0f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8a0f-107">Exchange コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-107">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="a8a0f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8a0f-108">Members</span></span>
|<span data-ttu-id="a8a0f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8a0f-109">Member</span></span>|<span data-ttu-id="a8a0f-110">値</span><span class="sxs-lookup"><span data-stu-id="a8a0f-110">Value</span></span>|<span data-ttu-id="a8a0f-111">説明</span><span class="sxs-lookup"><span data-stu-id="a8a0f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a0f-112">none</span><span class="sxs-lookup"><span data-stu-id="a8a0f-112">none</span></span>|<span data-ttu-id="a8a0f-113">0</span><span class="sxs-lookup"><span data-stu-id="a8a0f-113">0</span></span>|<span data-ttu-id="a8a0f-114">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-114">No Connector exists.</span></span>|
|<span data-ttu-id="a8a0f-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="a8a0f-115">connectionPending</span></span>|<span data-ttu-id="a8a0f-116">1</span><span class="sxs-lookup"><span data-stu-id="a8a0f-116">1</span></span>|<span data-ttu-id="a8a0f-117">Exchange 環境に対して保留中の接続です。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="a8a0f-118">接続されています。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-118">connected</span></span>|<span data-ttu-id="a8a0f-119">2</span><span class="sxs-lookup"><span data-stu-id="a8a0f-119">2</span></span>|<span data-ttu-id="a8a0f-120">Exchange 環境に接続されています。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="a8a0f-121">切断</span><span class="sxs-lookup"><span data-stu-id="a8a0f-121">disconnected</span></span>|<span data-ttu-id="a8a0f-122">3</span><span class="sxs-lookup"><span data-stu-id="a8a0f-122">3</span></span>|<span data-ttu-id="a8a0f-123">Exchange 環境から切断されています。</span><span class="sxs-lookup"><span data-stu-id="a8a0f-123">Disconnected from the Exchange Environment</span></span>|





