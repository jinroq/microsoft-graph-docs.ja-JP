---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
ms.openlocfilehash: 96117a7d11ca49cd39b60cb932bbb985ccf50d2a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069431"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="63ef5-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="63ef5-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="63ef5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="63ef5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63ef5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63ef5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63ef5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="63ef5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63ef5-107">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="63ef5-107">The type of Exchange Connector sync requested.</span></span>
## <a name="members"></a><span data-ttu-id="63ef5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="63ef5-108">Members</span></span>
|<span data-ttu-id="63ef5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="63ef5-109">Member</span></span>|<span data-ttu-id="63ef5-110">値</span><span class="sxs-lookup"><span data-stu-id="63ef5-110">Value</span></span>|<span data-ttu-id="63ef5-111">説明</span><span class="sxs-lookup"><span data-stu-id="63ef5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63ef5-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="63ef5-112">fullSync</span></span>|<span data-ttu-id="63ef5-113">0</span><span class="sxs-lookup"><span data-stu-id="63ef5-113">0</span></span>|<span data-ttu-id="63ef5-114">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="63ef5-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="63ef5-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="63ef5-115">deltaSync</span></span>|<span data-ttu-id="63ef5-116">1</span><span class="sxs-lookup"><span data-stu-id="63ef5-116">1</span></span>|<span data-ttu-id="63ef5-117">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="63ef5-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|





