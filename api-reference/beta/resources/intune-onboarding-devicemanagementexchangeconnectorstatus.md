---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange コネクタの現在の状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2d1bc97795a664515eb4ea6f620c41a64394be0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816059"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="0cd13-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="0cd13-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="0cd13-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0cd13-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cd13-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cd13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0cd13-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0cd13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cd13-107">Exchange コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="0cd13-107">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="0cd13-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0cd13-108">Members</span></span>
|<span data-ttu-id="0cd13-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="0cd13-109">Member</span></span>|<span data-ttu-id="0cd13-110">値</span><span class="sxs-lookup"><span data-stu-id="0cd13-110">Value</span></span>|<span data-ttu-id="0cd13-111">説明</span><span class="sxs-lookup"><span data-stu-id="0cd13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cd13-112">none</span><span class="sxs-lookup"><span data-stu-id="0cd13-112">none</span></span>|<span data-ttu-id="0cd13-113">0</span><span class="sxs-lookup"><span data-stu-id="0cd13-113">0</span></span>|<span data-ttu-id="0cd13-114">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="0cd13-114">No Connector exists.</span></span>|
|<span data-ttu-id="0cd13-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="0cd13-115">connectionPending</span></span>|<span data-ttu-id="0cd13-116">1</span><span class="sxs-lookup"><span data-stu-id="0cd13-116">1</span></span>|<span data-ttu-id="0cd13-117">Exchange 環境に対して保留中の接続です。</span><span class="sxs-lookup"><span data-stu-id="0cd13-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="0cd13-118">接続されています。</span><span class="sxs-lookup"><span data-stu-id="0cd13-118">connected</span></span>|<span data-ttu-id="0cd13-119">2</span><span class="sxs-lookup"><span data-stu-id="0cd13-119">2</span></span>|<span data-ttu-id="0cd13-120">Exchange 環境に接続されています。</span><span class="sxs-lookup"><span data-stu-id="0cd13-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="0cd13-121">切断</span><span class="sxs-lookup"><span data-stu-id="0cd13-121">disconnected</span></span>|<span data-ttu-id="0cd13-122">3</span><span class="sxs-lookup"><span data-stu-id="0cd13-122">3</span></span>|<span data-ttu-id="0cd13-123">Exchange 環境から切断されています。</span><span class="sxs-lookup"><span data-stu-id="0cd13-123">Disconnected from the Exchange Environment</span></span>|





