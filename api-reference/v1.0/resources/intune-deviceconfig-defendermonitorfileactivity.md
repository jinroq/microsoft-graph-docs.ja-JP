---
title: defenderMonitorFileActivity 列挙型
description: ファイル ・ アクティビティを監視するための可能な値です。
ms.openlocfilehash: 7784671f69712ce06a5aefa75048391cb097a89c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023955"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="a16c7-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="a16c7-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="a16c7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a16c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a16c7-105">ファイル ・ アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="a16c7-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="a16c7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a16c7-106">Members</span></span>
|<span data-ttu-id="a16c7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a16c7-107">Member</span></span>|<span data-ttu-id="a16c7-108">値</span><span class="sxs-lookup"><span data-stu-id="a16c7-108">Value</span></span>|<span data-ttu-id="a16c7-109">説明</span><span class="sxs-lookup"><span data-stu-id="a16c7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a16c7-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="a16c7-110">userDefined</span></span>|<span data-ttu-id="a16c7-111">0</span><span class="sxs-lookup"><span data-stu-id="a16c7-111">0</span></span>|<span data-ttu-id="a16c7-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="a16c7-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a16c7-113">無効にします。</span><span class="sxs-lookup"><span data-stu-id="a16c7-113">disable</span></span>|<span data-ttu-id="a16c7-114">1</span><span class="sxs-lookup"><span data-stu-id="a16c7-114">1</span></span>|<span data-ttu-id="a16c7-115">ファイル ・ アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="a16c7-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="a16c7-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="a16c7-116">monitorAllFiles</span></span>|<span data-ttu-id="a16c7-117">2</span><span class="sxs-lookup"><span data-stu-id="a16c7-117">2</span></span>|<span data-ttu-id="a16c7-118">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="a16c7-118">Monitor all files.</span></span>|
|<span data-ttu-id="a16c7-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="a16c7-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="a16c7-120">3</span><span class="sxs-lookup"><span data-stu-id="a16c7-120">3</span></span>| <span data-ttu-id="a16c7-121">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="a16c7-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="a16c7-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="a16c7-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="a16c7-123">4</span><span class="sxs-lookup"><span data-stu-id="a16c7-123">4</span></span>|<span data-ttu-id="a16c7-124">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="a16c7-124">Monitor outgoing files only.</span></span>|



