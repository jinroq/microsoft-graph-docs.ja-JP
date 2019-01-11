---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange コネクタの現在の状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c113a4d6af6493405a943384c2552f88a179ae5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840251"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="66b58-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="66b58-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="66b58-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="66b58-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66b58-105">Exchange コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="66b58-105">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="66b58-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="66b58-106">Members</span></span>
|<span data-ttu-id="66b58-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="66b58-107">Member</span></span>|<span data-ttu-id="66b58-108">値</span><span class="sxs-lookup"><span data-stu-id="66b58-108">Value</span></span>|<span data-ttu-id="66b58-109">説明</span><span class="sxs-lookup"><span data-stu-id="66b58-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66b58-110">none</span><span class="sxs-lookup"><span data-stu-id="66b58-110">none</span></span>|<span data-ttu-id="66b58-111">0</span><span class="sxs-lookup"><span data-stu-id="66b58-111">0</span></span>|<span data-ttu-id="66b58-112">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="66b58-112">No Connector exists.</span></span>|
|<span data-ttu-id="66b58-113">connectionPending</span><span class="sxs-lookup"><span data-stu-id="66b58-113">connectionPending</span></span>|<span data-ttu-id="66b58-114">1</span><span class="sxs-lookup"><span data-stu-id="66b58-114">1</span></span>|<span data-ttu-id="66b58-115">Exchange 環境に対して保留中の接続です。</span><span class="sxs-lookup"><span data-stu-id="66b58-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="66b58-116">接続されています。</span><span class="sxs-lookup"><span data-stu-id="66b58-116">connected</span></span>|<span data-ttu-id="66b58-117">2</span><span class="sxs-lookup"><span data-stu-id="66b58-117">2</span></span>|<span data-ttu-id="66b58-118">Exchange 環境に接続されています。</span><span class="sxs-lookup"><span data-stu-id="66b58-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="66b58-119">切断</span><span class="sxs-lookup"><span data-stu-id="66b58-119">disconnected</span></span>|<span data-ttu-id="66b58-120">3</span><span class="sxs-lookup"><span data-stu-id="66b58-120">3</span></span>|<span data-ttu-id="66b58-121">Exchange 環境から切断されています。</span><span class="sxs-lookup"><span data-stu-id="66b58-121">Disconnected from the Exchange Environment</span></span>|



