---
title: firewallPacketQueueingMethodType 列挙型
description: FirewallPacketQueueingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 49fdf3172879092a04c20d0d73724744a9ef0fb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031564"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="0e6c1-103">firewallPacketQueueingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0e6c1-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="0e6c1-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e6c1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e6c1-105">FirewallPacketQueueingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="0e6c1-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="0e6c1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0e6c1-106">Members</span></span>
|<span data-ttu-id="0e6c1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0e6c1-107">Member</span></span>|<span data-ttu-id="0e6c1-108">値</span><span class="sxs-lookup"><span data-stu-id="0e6c1-108">Value</span></span>|<span data-ttu-id="0e6c1-109">説明</span><span class="sxs-lookup"><span data-stu-id="0e6c1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e6c1-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="0e6c1-110">deviceDefault</span></span>|<span data-ttu-id="0e6c1-111">.0</span><span class="sxs-lookup"><span data-stu-id="0e6c1-111">0</span></span>|<span data-ttu-id="0e6c1-112">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="0e6c1-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="0e6c1-113">党</span><span class="sxs-lookup"><span data-stu-id="0e6c1-113">disabled</span></span>|<span data-ttu-id="0e6c1-114">1-d</span><span class="sxs-lookup"><span data-stu-id="0e6c1-114">1</span></span>|<span data-ttu-id="0e6c1-115">パケットキューを無効にする</span><span class="sxs-lookup"><span data-stu-id="0e6c1-115">Disable packet queuing</span></span>|
|<span data-ttu-id="0e6c1-116">queueInbound</span><span class="sxs-lookup"><span data-stu-id="0e6c1-116">queueInbound</span></span>|<span data-ttu-id="0e6c1-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0e6c1-117">2</span></span>|<span data-ttu-id="0e6c1-118">暗号化された着信パケットをキューに保存する</span><span class="sxs-lookup"><span data-stu-id="0e6c1-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="0e6c1-119">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="0e6c1-119">queueOutbound</span></span>|<span data-ttu-id="0e6c1-120">1/3</span><span class="sxs-lookup"><span data-stu-id="0e6c1-120">3</span></span>|<span data-ttu-id="0e6c1-121">転送のためにキューに復号化された送信パケット</span><span class="sxs-lookup"><span data-stu-id="0e6c1-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="0e6c1-122">queueBoth</span><span class="sxs-lookup"><span data-stu-id="0e6c1-122">queueBoth</span></span>|<span data-ttu-id="0e6c1-123">2/4</span><span class="sxs-lookup"><span data-stu-id="0e6c1-123">4</span></span>|<span data-ttu-id="0e6c1-124">受信パケットと送信パケットの両方をキューにする</span><span class="sxs-lookup"><span data-stu-id="0e6c1-124">Queue both inbound and outbound packets</span></span>|



