---
title: defenderMonitorFileActivity 列挙型
description: ファイル ・ アクティビティを監視するための可能な値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: df973c06456484263b6346b5eaa48ac466de41f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967995"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="d3de9-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="d3de9-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="d3de9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d3de9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3de9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3de9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3de9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3de9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3de9-107">ファイル ・ アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="d3de9-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="d3de9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3de9-108">Members</span></span>
|<span data-ttu-id="d3de9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3de9-109">Member</span></span>|<span data-ttu-id="d3de9-110">値</span><span class="sxs-lookup"><span data-stu-id="d3de9-110">Value</span></span>|<span data-ttu-id="d3de9-111">説明</span><span class="sxs-lookup"><span data-stu-id="d3de9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3de9-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="d3de9-112">userDefined</span></span>|<span data-ttu-id="d3de9-113">0</span><span class="sxs-lookup"><span data-stu-id="d3de9-113">0</span></span>|<span data-ttu-id="d3de9-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="d3de9-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d3de9-115">無効にします。</span><span class="sxs-lookup"><span data-stu-id="d3de9-115">disable</span></span>|<span data-ttu-id="d3de9-116">1</span><span class="sxs-lookup"><span data-stu-id="d3de9-116">1</span></span>|<span data-ttu-id="d3de9-117">ファイル ・ アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="d3de9-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="d3de9-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="d3de9-118">monitorAllFiles</span></span>|<span data-ttu-id="d3de9-119">2</span><span class="sxs-lookup"><span data-stu-id="d3de9-119">2</span></span>|<span data-ttu-id="d3de9-120">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="d3de9-120">Monitor all files.</span></span>|
|<span data-ttu-id="d3de9-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="d3de9-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="d3de9-122">3</span><span class="sxs-lookup"><span data-stu-id="d3de9-122">3</span></span>| <span data-ttu-id="d3de9-123">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="d3de9-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="d3de9-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="d3de9-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="d3de9-125">4</span><span class="sxs-lookup"><span data-stu-id="d3de9-125">4</span></span>|<span data-ttu-id="d3de9-126">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="d3de9-126">Monitor outgoing files only.</span></span>|





