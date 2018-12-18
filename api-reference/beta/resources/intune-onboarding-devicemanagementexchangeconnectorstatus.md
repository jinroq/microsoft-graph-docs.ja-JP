---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange コネクタの現在の状態です。
author: tfitzmac
ms.openlocfilehash: 7b2576d75eef285fe64e8ebf4d89dd004130fa78
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303795"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="ffc41-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="ffc41-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="ffc41-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ffc41-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffc41-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffc41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffc41-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ffc41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffc41-107">Exchange コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="ffc41-107">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="ffc41-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ffc41-108">Members</span></span>
|<span data-ttu-id="ffc41-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ffc41-109">Member</span></span>|<span data-ttu-id="ffc41-110">値</span><span class="sxs-lookup"><span data-stu-id="ffc41-110">Value</span></span>|<span data-ttu-id="ffc41-111">説明</span><span class="sxs-lookup"><span data-stu-id="ffc41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffc41-112">none</span><span class="sxs-lookup"><span data-stu-id="ffc41-112">none</span></span>|<span data-ttu-id="ffc41-113">0</span><span class="sxs-lookup"><span data-stu-id="ffc41-113">0</span></span>|<span data-ttu-id="ffc41-114">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="ffc41-114">No Connector exists.</span></span>|
|<span data-ttu-id="ffc41-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="ffc41-115">connectionPending</span></span>|<span data-ttu-id="ffc41-116">1</span><span class="sxs-lookup"><span data-stu-id="ffc41-116">1</span></span>|<span data-ttu-id="ffc41-117">Exchange 環境に対して保留中の接続です。</span><span class="sxs-lookup"><span data-stu-id="ffc41-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="ffc41-118">接続されています。</span><span class="sxs-lookup"><span data-stu-id="ffc41-118">connected</span></span>|<span data-ttu-id="ffc41-119">2</span><span class="sxs-lookup"><span data-stu-id="ffc41-119">2</span></span>|<span data-ttu-id="ffc41-120">Exchange 環境に接続されています。</span><span class="sxs-lookup"><span data-stu-id="ffc41-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="ffc41-121">切断</span><span class="sxs-lookup"><span data-stu-id="ffc41-121">disconnected</span></span>|<span data-ttu-id="ffc41-122">3</span><span class="sxs-lookup"><span data-stu-id="ffc41-122">3</span></span>|<span data-ttu-id="ffc41-123">Exchange 環境から切断されています。</span><span class="sxs-lookup"><span data-stu-id="ffc41-123">Disconnected from the Exchange Environment</span></span>|





