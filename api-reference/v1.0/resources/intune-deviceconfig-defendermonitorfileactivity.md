---
title: defenderMonitorFileActivity 列挙型
description: ファイル ・ アクティビティを監視するための可能な値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d818264470543d077384f055cf2ef4004e019b26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937118"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="e2a9c-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="e2a9c-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="e2a9c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e2a9c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2a9c-105">ファイル ・ アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="e2a9c-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="e2a9c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e2a9c-106">Members</span></span>
|<span data-ttu-id="e2a9c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e2a9c-107">Member</span></span>|<span data-ttu-id="e2a9c-108">値</span><span class="sxs-lookup"><span data-stu-id="e2a9c-108">Value</span></span>|<span data-ttu-id="e2a9c-109">説明</span><span class="sxs-lookup"><span data-stu-id="e2a9c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2a9c-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="e2a9c-110">userDefined</span></span>|<span data-ttu-id="e2a9c-111">0</span><span class="sxs-lookup"><span data-stu-id="e2a9c-111">0</span></span>|<span data-ttu-id="e2a9c-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="e2a9c-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e2a9c-113">無効にします。</span><span class="sxs-lookup"><span data-stu-id="e2a9c-113">disable</span></span>|<span data-ttu-id="e2a9c-114">1</span><span class="sxs-lookup"><span data-stu-id="e2a9c-114">1</span></span>|<span data-ttu-id="e2a9c-115">ファイル ・ アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="e2a9c-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="e2a9c-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="e2a9c-116">monitorAllFiles</span></span>|<span data-ttu-id="e2a9c-117">2</span><span class="sxs-lookup"><span data-stu-id="e2a9c-117">2</span></span>|<span data-ttu-id="e2a9c-118">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="e2a9c-118">Monitor all files.</span></span>|
|<span data-ttu-id="e2a9c-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="e2a9c-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="e2a9c-120">3</span><span class="sxs-lookup"><span data-stu-id="e2a9c-120">3</span></span>| <span data-ttu-id="e2a9c-121">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="e2a9c-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="e2a9c-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="e2a9c-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="e2a9c-123">4</span><span class="sxs-lookup"><span data-stu-id="e2a9c-123">4</span></span>|<span data-ttu-id="e2a9c-124">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="e2a9c-124">Monitor outgoing files only.</span></span>|



