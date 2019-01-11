---
title: defenderMonitorFileActivity 列挙型
description: ファイル ・ アクティビティを監視するための可能な値です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e8719fd5f07efa9d09dcf88ae02566f331904734
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871688"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="d4649-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="d4649-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="d4649-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4649-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4649-105">ファイル ・ アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="d4649-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="d4649-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d4649-106">Members</span></span>
|<span data-ttu-id="d4649-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d4649-107">Member</span></span>|<span data-ttu-id="d4649-108">値</span><span class="sxs-lookup"><span data-stu-id="d4649-108">Value</span></span>|<span data-ttu-id="d4649-109">説明</span><span class="sxs-lookup"><span data-stu-id="d4649-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4649-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="d4649-110">userDefined</span></span>|<span data-ttu-id="d4649-111">0</span><span class="sxs-lookup"><span data-stu-id="d4649-111">0</span></span>|<span data-ttu-id="d4649-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="d4649-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d4649-113">無効にします。</span><span class="sxs-lookup"><span data-stu-id="d4649-113">disable</span></span>|<span data-ttu-id="d4649-114">1</span><span class="sxs-lookup"><span data-stu-id="d4649-114">1</span></span>|<span data-ttu-id="d4649-115">ファイル ・ アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="d4649-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="d4649-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="d4649-116">monitorAllFiles</span></span>|<span data-ttu-id="d4649-117">2</span><span class="sxs-lookup"><span data-stu-id="d4649-117">2</span></span>|<span data-ttu-id="d4649-118">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="d4649-118">Monitor all files.</span></span>|
|<span data-ttu-id="d4649-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="d4649-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="d4649-120">3</span><span class="sxs-lookup"><span data-stu-id="d4649-120">3</span></span>| <span data-ttu-id="d4649-121">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="d4649-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="d4649-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="d4649-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="d4649-123">4</span><span class="sxs-lookup"><span data-stu-id="d4649-123">4</span></span>|<span data-ttu-id="d4649-124">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="d4649-124">Monitor outgoing files only.</span></span>|



