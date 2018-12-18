---
title: defenderMonitorFileActivity 列挙型
description: ファイル ・ アクティビティを監視するための可能な値です。
author: tfitzmac
ms.openlocfilehash: 87c8656c09482763b5e09f0ca746c7bddd069a21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314764"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="637dc-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="637dc-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="637dc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="637dc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="637dc-105">ファイル ・ アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="637dc-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="637dc-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="637dc-106">Members</span></span>
|<span data-ttu-id="637dc-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="637dc-107">Member</span></span>|<span data-ttu-id="637dc-108">値</span><span class="sxs-lookup"><span data-stu-id="637dc-108">Value</span></span>|<span data-ttu-id="637dc-109">説明</span><span class="sxs-lookup"><span data-stu-id="637dc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="637dc-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="637dc-110">userDefined</span></span>|<span data-ttu-id="637dc-111">0</span><span class="sxs-lookup"><span data-stu-id="637dc-111">0</span></span>|<span data-ttu-id="637dc-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="637dc-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="637dc-113">無効にします。</span><span class="sxs-lookup"><span data-stu-id="637dc-113">disable</span></span>|<span data-ttu-id="637dc-114">1</span><span class="sxs-lookup"><span data-stu-id="637dc-114">1</span></span>|<span data-ttu-id="637dc-115">ファイル ・ アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="637dc-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="637dc-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="637dc-116">monitorAllFiles</span></span>|<span data-ttu-id="637dc-117">2</span><span class="sxs-lookup"><span data-stu-id="637dc-117">2</span></span>|<span data-ttu-id="637dc-118">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="637dc-118">Monitor all files.</span></span>|
|<span data-ttu-id="637dc-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="637dc-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="637dc-120">3</span><span class="sxs-lookup"><span data-stu-id="637dc-120">3</span></span>| <span data-ttu-id="637dc-121">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="637dc-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="637dc-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="637dc-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="637dc-123">4</span><span class="sxs-lookup"><span data-stu-id="637dc-123">4</span></span>|<span data-ttu-id="637dc-124">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="637dc-124">Monitor outgoing files only.</span></span>|



