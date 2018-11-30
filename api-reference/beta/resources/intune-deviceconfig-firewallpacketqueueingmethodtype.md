---
title: firewallPacketQueueingMethodType 列挙型
description: FirewallPacketQueueingMethod に指定できる値
ms.openlocfilehash: f55b68780d3bec97fa48a32c7abd8e1cfb269755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071606"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="742a7-103">firewallPacketQueueingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="742a7-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="742a7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="742a7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="742a7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="742a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="742a7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="742a7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="742a7-107">FirewallPacketQueueingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="742a7-107">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="742a7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="742a7-108">Members</span></span>
|<span data-ttu-id="742a7-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="742a7-109">Member</span></span>|<span data-ttu-id="742a7-110">値</span><span class="sxs-lookup"><span data-stu-id="742a7-110">Value</span></span>|<span data-ttu-id="742a7-111">説明</span><span class="sxs-lookup"><span data-stu-id="742a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="742a7-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="742a7-112">deviceDefault</span></span>|<span data-ttu-id="742a7-113">0</span><span class="sxs-lookup"><span data-stu-id="742a7-113">0</span></span>|<span data-ttu-id="742a7-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="742a7-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="742a7-115">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="742a7-115">disabled</span></span>|<span data-ttu-id="742a7-116">1</span><span class="sxs-lookup"><span data-stu-id="742a7-116">1</span></span>|<span data-ttu-id="742a7-117">パケットのキューを無効にします。</span><span class="sxs-lookup"><span data-stu-id="742a7-117">Disable packet queuing</span></span>|
|<span data-ttu-id="742a7-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="742a7-118">queueInbound</span></span>|<span data-ttu-id="742a7-119">2</span><span class="sxs-lookup"><span data-stu-id="742a7-119">2</span></span>|<span data-ttu-id="742a7-120">キューが暗号化されたパケットを受信</span><span class="sxs-lookup"><span data-stu-id="742a7-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="742a7-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="742a7-121">queueOutbound</span></span>|<span data-ttu-id="742a7-122">3</span><span class="sxs-lookup"><span data-stu-id="742a7-122">3</span></span>|<span data-ttu-id="742a7-123">キューは、転送のためのアウト バウンド パケットを復号化</span><span class="sxs-lookup"><span data-stu-id="742a7-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="742a7-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="742a7-124">queueBoth</span></span>|<span data-ttu-id="742a7-125">4</span><span class="sxs-lookup"><span data-stu-id="742a7-125">4</span></span>|<span data-ttu-id="742a7-126">着信および発信パケットをキューします。</span><span class="sxs-lookup"><span data-stu-id="742a7-126">Queue both inbound and outbound packets</span></span>|





