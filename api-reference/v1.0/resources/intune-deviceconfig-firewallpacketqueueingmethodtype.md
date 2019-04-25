---
title: firewallPacketQueueingMethodType 列挙型
description: firewallPacketQueueingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd9dc0279abc332bbf7b686f7f429fbd8db8883
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541309"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="2aa25-103">firewallPacketQueueingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="2aa25-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="2aa25-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2aa25-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aa25-105">firewallPacketQueueingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="2aa25-105">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="2aa25-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="2aa25-106">Members</span></span>
|<span data-ttu-id="2aa25-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2aa25-107">Member</span></span>|<span data-ttu-id="2aa25-108">値</span><span class="sxs-lookup"><span data-stu-id="2aa25-108">Value</span></span>|<span data-ttu-id="2aa25-109">説明</span><span class="sxs-lookup"><span data-stu-id="2aa25-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aa25-110">devicedefault</span><span class="sxs-lookup"><span data-stu-id="2aa25-110">deviceDefault</span></span>|<span data-ttu-id="2aa25-111">.0</span><span class="sxs-lookup"><span data-stu-id="2aa25-111">0</span></span>|<span data-ttu-id="2aa25-112">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="2aa25-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="2aa25-113">党</span><span class="sxs-lookup"><span data-stu-id="2aa25-113">disabled</span></span>|<span data-ttu-id="2aa25-114">1 </span><span class="sxs-lookup"><span data-stu-id="2aa25-114">1</span></span>|<span data-ttu-id="2aa25-115">パケットキューを無効にする</span><span class="sxs-lookup"><span data-stu-id="2aa25-115">Disable packet queuing</span></span>|
|<span data-ttu-id="2aa25-116">queueinbound</span><span class="sxs-lookup"><span data-stu-id="2aa25-116">queueInbound</span></span>|<span data-ttu-id="2aa25-117">2 </span><span class="sxs-lookup"><span data-stu-id="2aa25-117">2</span></span>|<span data-ttu-id="2aa25-118">暗号化された着信パケットをキューに保存する</span><span class="sxs-lookup"><span data-stu-id="2aa25-118">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="2aa25-119">queueoutbound</span><span class="sxs-lookup"><span data-stu-id="2aa25-119">queueOutbound</span></span>|<span data-ttu-id="2aa25-120">3 </span><span class="sxs-lookup"><span data-stu-id="2aa25-120">3</span></span>|<span data-ttu-id="2aa25-121">転送のためにキューに復号化された送信パケット</span><span class="sxs-lookup"><span data-stu-id="2aa25-121">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="2aa25-122">queueboth</span><span class="sxs-lookup"><span data-stu-id="2aa25-122">queueBoth</span></span>|<span data-ttu-id="2aa25-123">4 </span><span class="sxs-lookup"><span data-stu-id="2aa25-123">4</span></span>|<span data-ttu-id="2aa25-124">受信パケットと送信パケットの両方をキューにする</span><span class="sxs-lookup"><span data-stu-id="2aa25-124">Queue both inbound and outbound packets</span></span>|



