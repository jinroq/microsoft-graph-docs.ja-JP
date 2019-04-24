---
title: firewallPacketQueueingMethodType 列挙型
description: firewallPacketQueueingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2b83aa5d13ac170df1f9f99f8e430d10cdaba3e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460584"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="81e27-103">firewallPacketQueueingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="81e27-103">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="81e27-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81e27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81e27-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81e27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81e27-106">firewallPacketQueueingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="81e27-106">Possible values for firewallPacketQueueingMethod</span></span>

## <a name="members"></a><span data-ttu-id="81e27-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="81e27-107">Members</span></span>
|<span data-ttu-id="81e27-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="81e27-108">Member</span></span>|<span data-ttu-id="81e27-109">値</span><span class="sxs-lookup"><span data-stu-id="81e27-109">Value</span></span>|<span data-ttu-id="81e27-110">説明</span><span class="sxs-lookup"><span data-stu-id="81e27-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81e27-111">devicedefault</span><span class="sxs-lookup"><span data-stu-id="81e27-111">deviceDefault</span></span>|<span data-ttu-id="81e27-112">.0</span><span class="sxs-lookup"><span data-stu-id="81e27-112">0</span></span>|<span data-ttu-id="81e27-113">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="81e27-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="81e27-114">党</span><span class="sxs-lookup"><span data-stu-id="81e27-114">disabled</span></span>|<span data-ttu-id="81e27-115">1-d</span><span class="sxs-lookup"><span data-stu-id="81e27-115">1</span></span>|<span data-ttu-id="81e27-116">パケットキューを無効にする</span><span class="sxs-lookup"><span data-stu-id="81e27-116">Disable packet queuing</span></span>|
|<span data-ttu-id="81e27-117">queueinbound</span><span class="sxs-lookup"><span data-stu-id="81e27-117">queueInbound</span></span>|<span data-ttu-id="81e27-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="81e27-118">2</span></span>|<span data-ttu-id="81e27-119">暗号化された着信パケットをキューに保存する</span><span class="sxs-lookup"><span data-stu-id="81e27-119">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="81e27-120">queueoutbound</span><span class="sxs-lookup"><span data-stu-id="81e27-120">queueOutbound</span></span>|<span data-ttu-id="81e27-121">1/3</span><span class="sxs-lookup"><span data-stu-id="81e27-121">3</span></span>|<span data-ttu-id="81e27-122">転送のためにキューに復号化された送信パケット</span><span class="sxs-lookup"><span data-stu-id="81e27-122">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="81e27-123">queueboth</span><span class="sxs-lookup"><span data-stu-id="81e27-123">queueBoth</span></span>|<span data-ttu-id="81e27-124">2/4</span><span class="sxs-lookup"><span data-stu-id="81e27-124">4</span></span>|<span data-ttu-id="81e27-125">受信パケットと送信パケットの両方をキューにする</span><span class="sxs-lookup"><span data-stu-id="81e27-125">Queue both inbound and outbound packets</span></span>|





