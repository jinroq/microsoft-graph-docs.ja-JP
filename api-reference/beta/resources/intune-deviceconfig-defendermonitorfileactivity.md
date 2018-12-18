---
title: defenderMonitorFileActivity 列挙型
description: ファイル ・ アクティビティを監視するための可能な値です。
author: tfitzmac
ms.openlocfilehash: 32b3972f6c4c09117f3b8001038c0316235ea222
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338109"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="2b884-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="2b884-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="2b884-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b884-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b884-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b884-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b884-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b884-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b884-107">ファイル ・ アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="2b884-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="2b884-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2b884-108">Members</span></span>
|<span data-ttu-id="2b884-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="2b884-109">Member</span></span>|<span data-ttu-id="2b884-110">値</span><span class="sxs-lookup"><span data-stu-id="2b884-110">Value</span></span>|<span data-ttu-id="2b884-111">説明</span><span class="sxs-lookup"><span data-stu-id="2b884-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b884-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="2b884-112">userDefined</span></span>|<span data-ttu-id="2b884-113">0</span><span class="sxs-lookup"><span data-stu-id="2b884-113">0</span></span>|<span data-ttu-id="2b884-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="2b884-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2b884-115">無効にします。</span><span class="sxs-lookup"><span data-stu-id="2b884-115">disable</span></span>|<span data-ttu-id="2b884-116">1</span><span class="sxs-lookup"><span data-stu-id="2b884-116">1</span></span>|<span data-ttu-id="2b884-117">ファイル ・ アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="2b884-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="2b884-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="2b884-118">monitorAllFiles</span></span>|<span data-ttu-id="2b884-119">2</span><span class="sxs-lookup"><span data-stu-id="2b884-119">2</span></span>|<span data-ttu-id="2b884-120">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="2b884-120">Monitor all files.</span></span>|
|<span data-ttu-id="2b884-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="2b884-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="2b884-122">3</span><span class="sxs-lookup"><span data-stu-id="2b884-122">3</span></span>| <span data-ttu-id="2b884-123">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="2b884-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="2b884-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="2b884-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="2b884-125">4</span><span class="sxs-lookup"><span data-stu-id="2b884-125">4</span></span>|<span data-ttu-id="2b884-126">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="2b884-126">Monitor outgoing files only.</span></span>|





