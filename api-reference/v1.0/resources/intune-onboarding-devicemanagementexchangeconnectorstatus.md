---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange コネクタの現在の状態です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42a7d99a4b19505e999f8a3aeea48829ee4aa987
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917665"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="769b0-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="769b0-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="769b0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="769b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="769b0-105">Exchange コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="769b0-105">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="769b0-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="769b0-106">Members</span></span>
|<span data-ttu-id="769b0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="769b0-107">Member</span></span>|<span data-ttu-id="769b0-108">値</span><span class="sxs-lookup"><span data-stu-id="769b0-108">Value</span></span>|<span data-ttu-id="769b0-109">説明</span><span class="sxs-lookup"><span data-stu-id="769b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="769b0-110">none</span><span class="sxs-lookup"><span data-stu-id="769b0-110">none</span></span>|<span data-ttu-id="769b0-111">0</span><span class="sxs-lookup"><span data-stu-id="769b0-111">0</span></span>|<span data-ttu-id="769b0-112">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="769b0-112">No Connector exists.</span></span>|
|<span data-ttu-id="769b0-113">connectionPending</span><span class="sxs-lookup"><span data-stu-id="769b0-113">connectionPending</span></span>|<span data-ttu-id="769b0-114">1</span><span class="sxs-lookup"><span data-stu-id="769b0-114">1</span></span>|<span data-ttu-id="769b0-115">Exchange 環境に対して保留中の接続です。</span><span class="sxs-lookup"><span data-stu-id="769b0-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="769b0-116">接続されています。</span><span class="sxs-lookup"><span data-stu-id="769b0-116">connected</span></span>|<span data-ttu-id="769b0-117">2</span><span class="sxs-lookup"><span data-stu-id="769b0-117">2</span></span>|<span data-ttu-id="769b0-118">Exchange 環境に接続されています。</span><span class="sxs-lookup"><span data-stu-id="769b0-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="769b0-119">切断</span><span class="sxs-lookup"><span data-stu-id="769b0-119">disconnected</span></span>|<span data-ttu-id="769b0-120">3</span><span class="sxs-lookup"><span data-stu-id="769b0-120">3</span></span>|<span data-ttu-id="769b0-121">Exchange 環境から切断されています。</span><span class="sxs-lookup"><span data-stu-id="769b0-121">Disconnected from the Exchange Environment</span></span>|



