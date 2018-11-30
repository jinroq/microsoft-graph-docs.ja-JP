---
title: firewallPacketQueueingMethodType 列挙型
description: FirewallPacketQueueingMethod に指定できる値
ms.openlocfilehash: 70643e300f1a6cc151edeae849e5ae7c5f977750
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022414"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="68408-103">firewallPacketQueueingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="68408-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="68408-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68408-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68408-105">FirewallPacketQueueingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="68408-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="68408-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="68408-106">Members</span></span>
|<span data-ttu-id="68408-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="68408-107">Member</span></span>|<span data-ttu-id="68408-108">値</span><span class="sxs-lookup"><span data-stu-id="68408-108">Value</span></span>|<span data-ttu-id="68408-109">説明</span><span class="sxs-lookup"><span data-stu-id="68408-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68408-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="68408-110">deviceDefault</span></span>|<span data-ttu-id="68408-111">0</span><span class="sxs-lookup"><span data-stu-id="68408-111">0</span></span>|<span data-ttu-id="68408-112">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="68408-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="68408-113">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="68408-113">disabled</span></span>|<span data-ttu-id="68408-114">1</span><span class="sxs-lookup"><span data-stu-id="68408-114">1</span></span>|<span data-ttu-id="68408-115">パケットのキューを無効にします。</span><span class="sxs-lookup"><span data-stu-id="68408-115">Disable packet queuing</span></span>|
|<span data-ttu-id="68408-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="68408-116">queueInbound</span></span>|<span data-ttu-id="68408-117">2</span><span class="sxs-lookup"><span data-stu-id="68408-117">2</span></span>|<span data-ttu-id="68408-118">キューが暗号化されたパケットを受信</span><span class="sxs-lookup"><span data-stu-id="68408-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="68408-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="68408-119">queueOutbound</span></span>|<span data-ttu-id="68408-120">3</span><span class="sxs-lookup"><span data-stu-id="68408-120">3</span></span>|<span data-ttu-id="68408-121">キューは、転送のためのアウト バウンド パケットを復号化</span><span class="sxs-lookup"><span data-stu-id="68408-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="68408-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="68408-122">queueBoth</span></span>|<span data-ttu-id="68408-123">4</span><span class="sxs-lookup"><span data-stu-id="68408-123">4</span></span>|<span data-ttu-id="68408-124">着信および発信パケットをキューします。</span><span class="sxs-lookup"><span data-stu-id="68408-124">Queue both inbound and outbound packets</span></span>|



