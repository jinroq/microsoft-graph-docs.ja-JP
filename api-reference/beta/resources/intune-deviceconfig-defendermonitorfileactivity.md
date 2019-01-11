---
title: defenderMonitorFileActivity 列挙型
description: ファイル ・ アクティビティを監視するための可能な値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1d7b6c921ec40b53339646b2b3b0a91e2d4e8a84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837906"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="69a3a-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="69a3a-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="69a3a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="69a3a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69a3a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69a3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69a3a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="69a3a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69a3a-107">ファイル ・ アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="69a3a-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="69a3a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="69a3a-108">Members</span></span>
|<span data-ttu-id="69a3a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="69a3a-109">Member</span></span>|<span data-ttu-id="69a3a-110">値</span><span class="sxs-lookup"><span data-stu-id="69a3a-110">Value</span></span>|<span data-ttu-id="69a3a-111">説明</span><span class="sxs-lookup"><span data-stu-id="69a3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69a3a-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="69a3a-112">userDefined</span></span>|<span data-ttu-id="69a3a-113">0</span><span class="sxs-lookup"><span data-stu-id="69a3a-113">0</span></span>|<span data-ttu-id="69a3a-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="69a3a-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="69a3a-115">無効にします。</span><span class="sxs-lookup"><span data-stu-id="69a3a-115">disable</span></span>|<span data-ttu-id="69a3a-116">1</span><span class="sxs-lookup"><span data-stu-id="69a3a-116">1</span></span>|<span data-ttu-id="69a3a-117">ファイル ・ アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="69a3a-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="69a3a-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="69a3a-118">monitorAllFiles</span></span>|<span data-ttu-id="69a3a-119">2</span><span class="sxs-lookup"><span data-stu-id="69a3a-119">2</span></span>|<span data-ttu-id="69a3a-120">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="69a3a-120">Monitor all files.</span></span>|
|<span data-ttu-id="69a3a-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="69a3a-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="69a3a-122">3</span><span class="sxs-lookup"><span data-stu-id="69a3a-122">3</span></span>| <span data-ttu-id="69a3a-123">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="69a3a-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="69a3a-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="69a3a-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="69a3a-125">4</span><span class="sxs-lookup"><span data-stu-id="69a3a-125">4</span></span>|<span data-ttu-id="69a3a-126">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="69a3a-126">Monitor outgoing files only.</span></span>|





