---
title: firewallPacketQueueingMethodType 列挙型
description: FirewallPacketQueueingMethod に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4222580a079fd37b381cdaf78e0b2985029ef34b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338141"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="f8dee-103">firewallPacketQueueingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f8dee-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="f8dee-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f8dee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8dee-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f8dee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8dee-106">FirewallPacketQueueingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="f8dee-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="f8dee-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8dee-107">Members</span></span>
|<span data-ttu-id="f8dee-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f8dee-108">Member</span></span>|<span data-ttu-id="f8dee-109">値</span><span class="sxs-lookup"><span data-stu-id="f8dee-109">Value</span></span>|<span data-ttu-id="f8dee-110">説明</span><span class="sxs-lookup"><span data-stu-id="f8dee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8dee-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f8dee-111">deviceDefault</span></span>|<span data-ttu-id="f8dee-112">.0</span><span class="sxs-lookup"><span data-stu-id="f8dee-112">0</span></span>|<span data-ttu-id="f8dee-113">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="f8dee-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f8dee-114">党</span><span class="sxs-lookup"><span data-stu-id="f8dee-114">disabled</span></span>|<span data-ttu-id="f8dee-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f8dee-115">1</span></span>|<span data-ttu-id="f8dee-116">パケットキューを無効にする</span><span class="sxs-lookup"><span data-stu-id="f8dee-116">Disable packet queuing</span></span>|
|<span data-ttu-id="f8dee-117">queueInbound</span><span class="sxs-lookup"><span data-stu-id="f8dee-117">queueInbound</span></span>|<span data-ttu-id="f8dee-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f8dee-118">2</span></span>|<span data-ttu-id="f8dee-119">暗号化された着信パケットをキューに保存する</span><span class="sxs-lookup"><span data-stu-id="f8dee-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="f8dee-120">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="f8dee-120">queueOutbound</span></span>|<span data-ttu-id="f8dee-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f8dee-121">3</span></span>|<span data-ttu-id="f8dee-122">転送のためにキューに復号化された送信パケット</span><span class="sxs-lookup"><span data-stu-id="f8dee-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="f8dee-123">queueBoth</span><span class="sxs-lookup"><span data-stu-id="f8dee-123">queueBoth</span></span>|<span data-ttu-id="f8dee-124">2/4</span><span class="sxs-lookup"><span data-stu-id="f8dee-124">4</span></span>|<span data-ttu-id="f8dee-125">受信パケットと送信パケットの両方をキューにする</span><span class="sxs-lookup"><span data-stu-id="f8dee-125">Queue both inbound and outbound packets</span></span>|



