---
title: firewallPacketQueueingMethodType 列挙型
description: FirewallPacketQueueingMethod に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dc40b93eebc17b1d1abcd9c317da1ffa538512a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425758"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="ec103-103">firewallPacketQueueingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ec103-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="ec103-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ec103-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ec103-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec103-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec103-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec103-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec103-107">FirewallPacketQueueingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="ec103-107">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="ec103-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec103-108">Members</span></span>
|<span data-ttu-id="ec103-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ec103-109">Member</span></span>|<span data-ttu-id="ec103-110">値</span><span class="sxs-lookup"><span data-stu-id="ec103-110">Value</span></span>|<span data-ttu-id="ec103-111">説明</span><span class="sxs-lookup"><span data-stu-id="ec103-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec103-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ec103-112">deviceDefault</span></span>|<span data-ttu-id="ec103-113">0</span><span class="sxs-lookup"><span data-stu-id="ec103-113">0</span></span>|<span data-ttu-id="ec103-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="ec103-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ec103-115">無効になっています。</span><span class="sxs-lookup"><span data-stu-id="ec103-115">disabled</span></span>|<span data-ttu-id="ec103-116">1</span><span class="sxs-lookup"><span data-stu-id="ec103-116">1</span></span>|<span data-ttu-id="ec103-117">パケットのキューを無効にします。</span><span class="sxs-lookup"><span data-stu-id="ec103-117">Disable packet queuing</span></span>|
|<span data-ttu-id="ec103-118">queueInbound</span><span class="sxs-lookup"><span data-stu-id="ec103-118">queueInbound</span></span>|<span data-ttu-id="ec103-119">2</span><span class="sxs-lookup"><span data-stu-id="ec103-119">2</span></span>|<span data-ttu-id="ec103-120">キューが暗号化されたパケットを受信</span><span class="sxs-lookup"><span data-stu-id="ec103-120">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="ec103-121">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="ec103-121">queueOutbound</span></span>|<span data-ttu-id="ec103-122">3</span><span class="sxs-lookup"><span data-stu-id="ec103-122">3</span></span>|<span data-ttu-id="ec103-123">キューは、転送のためのアウト バウンド パケットを復号化</span><span class="sxs-lookup"><span data-stu-id="ec103-123">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="ec103-124">queueBoth</span><span class="sxs-lookup"><span data-stu-id="ec103-124">queueBoth</span></span>|<span data-ttu-id="ec103-125">4</span><span class="sxs-lookup"><span data-stu-id="ec103-125">4</span></span>|<span data-ttu-id="ec103-126">着信および発信パケットをキューします。</span><span class="sxs-lookup"><span data-stu-id="ec103-126">Queue both inbound and outbound packets</span></span>|




