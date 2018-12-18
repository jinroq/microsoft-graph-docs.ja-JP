---
title: firewallPacketQueueingMethodType 列挙型
description: FirewallPacketQueueingMethod に指定できる値
author: tfitzmac
ms.openlocfilehash: 9f3d63b7e58b6f9c5ba369c3ceb12d06704c4725
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304558"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="d9df4-103">firewallPacketQueueingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d9df4-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="d9df4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d9df4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9df4-105">FirewallPacketQueueingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="d9df4-105">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="d9df4-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9df4-106">Members</span></span>
|<span data-ttu-id="d9df4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d9df4-107">Member</span></span>|<span data-ttu-id="d9df4-108">値</span><span class="sxs-lookup"><span data-stu-id="d9df4-108">Value</span></span>|<span data-ttu-id="d9df4-109">説明</span><span class="sxs-lookup"><span data-stu-id="d9df4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9df4-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d9df4-110">deviceDefault</span></span>|<span data-ttu-id="d9df4-111">0</span><span class="sxs-lookup"><span data-stu-id="d9df4-111">0</span></span>|<span data-ttu-id="d9df4-112">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="d9df4-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d9df4-113">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="d9df4-113">disabled</span></span>|<span data-ttu-id="d9df4-114">1</span><span class="sxs-lookup"><span data-stu-id="d9df4-114">1</span></span>|<span data-ttu-id="d9df4-115">パケットのキューを無効にします。</span><span class="sxs-lookup"><span data-stu-id="d9df4-115">Disable packet queuing</span></span>|
|<span data-ttu-id="d9df4-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="d9df4-116">queueInbound</span></span>|<span data-ttu-id="d9df4-117">2</span><span class="sxs-lookup"><span data-stu-id="d9df4-117">2</span></span>|<span data-ttu-id="d9df4-118">キューが暗号化されたパケットを受信</span><span class="sxs-lookup"><span data-stu-id="d9df4-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="d9df4-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="d9df4-119">queueOutbound</span></span>|<span data-ttu-id="d9df4-120">3</span><span class="sxs-lookup"><span data-stu-id="d9df4-120">3</span></span>|<span data-ttu-id="d9df4-121">キューは、転送のためのアウト バウンド パケットを復号化</span><span class="sxs-lookup"><span data-stu-id="d9df4-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="d9df4-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="d9df4-122">queueBoth</span></span>|<span data-ttu-id="d9df4-123">4</span><span class="sxs-lookup"><span data-stu-id="d9df4-123">4</span></span>|<span data-ttu-id="d9df4-124">着信および発信パケットをキューします。</span><span class="sxs-lookup"><span data-stu-id="d9df4-124">Queue both inbound and outbound packets</span></span>|



