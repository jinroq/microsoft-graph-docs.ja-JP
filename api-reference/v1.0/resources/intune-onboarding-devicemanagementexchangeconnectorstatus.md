---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange コネクタの現在の状態です。
author: tfitzmac
ms.openlocfilehash: 6655e4c659141558d0c1e873f0e17ee3439ea95b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330668"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="27bdc-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="27bdc-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="27bdc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="27bdc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27bdc-105">Exchange コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="27bdc-105">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="27bdc-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="27bdc-106">Members</span></span>
|<span data-ttu-id="27bdc-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="27bdc-107">Member</span></span>|<span data-ttu-id="27bdc-108">値</span><span class="sxs-lookup"><span data-stu-id="27bdc-108">Value</span></span>|<span data-ttu-id="27bdc-109">説明</span><span class="sxs-lookup"><span data-stu-id="27bdc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27bdc-110">none</span><span class="sxs-lookup"><span data-stu-id="27bdc-110">none</span></span>|<span data-ttu-id="27bdc-111">0</span><span class="sxs-lookup"><span data-stu-id="27bdc-111">0</span></span>|<span data-ttu-id="27bdc-112">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="27bdc-112">No Connector exists.</span></span>|
|<span data-ttu-id="27bdc-113">connectionPending</span><span class="sxs-lookup"><span data-stu-id="27bdc-113">connectionPending</span></span>|<span data-ttu-id="27bdc-114">1</span><span class="sxs-lookup"><span data-stu-id="27bdc-114">1</span></span>|<span data-ttu-id="27bdc-115">Exchange 環境に対して保留中の接続です。</span><span class="sxs-lookup"><span data-stu-id="27bdc-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="27bdc-116">接続されています。</span><span class="sxs-lookup"><span data-stu-id="27bdc-116">connected</span></span>|<span data-ttu-id="27bdc-117">2</span><span class="sxs-lookup"><span data-stu-id="27bdc-117">2</span></span>|<span data-ttu-id="27bdc-118">Exchange 環境に接続されています。</span><span class="sxs-lookup"><span data-stu-id="27bdc-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="27bdc-119">切断</span><span class="sxs-lookup"><span data-stu-id="27bdc-119">disconnected</span></span>|<span data-ttu-id="27bdc-120">3</span><span class="sxs-lookup"><span data-stu-id="27bdc-120">3</span></span>|<span data-ttu-id="27bdc-121">Exchange 環境から切断されています。</span><span class="sxs-lookup"><span data-stu-id="27bdc-121">Disconnected from the Exchange Environment</span></span>|



