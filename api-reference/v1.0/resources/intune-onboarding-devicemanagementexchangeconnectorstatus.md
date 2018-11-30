---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange コネクタの現在の状態です。
ms.openlocfilehash: 2ff80dde75889ce2380d6e365aaec871b85afd81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021722"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="72532-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="72532-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="72532-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="72532-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72532-105">Exchange コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="72532-105">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="72532-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="72532-106">Members</span></span>
|<span data-ttu-id="72532-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="72532-107">Member</span></span>|<span data-ttu-id="72532-108">値</span><span class="sxs-lookup"><span data-stu-id="72532-108">Value</span></span>|<span data-ttu-id="72532-109">説明</span><span class="sxs-lookup"><span data-stu-id="72532-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72532-110">none</span><span class="sxs-lookup"><span data-stu-id="72532-110">none</span></span>|<span data-ttu-id="72532-111">0</span><span class="sxs-lookup"><span data-stu-id="72532-111">0</span></span>|<span data-ttu-id="72532-112">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="72532-112">No Connector exists.</span></span>|
|<span data-ttu-id="72532-113">connectionPending</span><span class="sxs-lookup"><span data-stu-id="72532-113">connectionPending</span></span>|<span data-ttu-id="72532-114">1</span><span class="sxs-lookup"><span data-stu-id="72532-114">1</span></span>|<span data-ttu-id="72532-115">Exchange 環境に対して保留中の接続です。</span><span class="sxs-lookup"><span data-stu-id="72532-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="72532-116">接続されています。</span><span class="sxs-lookup"><span data-stu-id="72532-116">connected</span></span>|<span data-ttu-id="72532-117">2</span><span class="sxs-lookup"><span data-stu-id="72532-117">2</span></span>|<span data-ttu-id="72532-118">Exchange 環境に接続されています。</span><span class="sxs-lookup"><span data-stu-id="72532-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="72532-119">切断</span><span class="sxs-lookup"><span data-stu-id="72532-119">disconnected</span></span>|<span data-ttu-id="72532-120">3</span><span class="sxs-lookup"><span data-stu-id="72532-120">3</span></span>|<span data-ttu-id="72532-121">Exchange 環境から切断されています。</span><span class="sxs-lookup"><span data-stu-id="72532-121">Disconnected from the Exchange Environment</span></span>|



