---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cba0a3fcd25c9f4672d7590718c25e977edf635b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949144"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="e8bf2-103">applicationGuardBlockClipboardSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e8bf2-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="e8bf2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8bf2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8bf2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8bf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8bf2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8bf2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8bf2-107">ApplicationGuardBlockClipboardSharingType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="e8bf2-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="e8bf2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e8bf2-108">Members</span></span>
|<span data-ttu-id="e8bf2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e8bf2-109">Member</span></span>|<span data-ttu-id="e8bf2-110">値</span><span class="sxs-lookup"><span data-stu-id="e8bf2-110">Value</span></span>|<span data-ttu-id="e8bf2-111">説明</span><span class="sxs-lookup"><span data-stu-id="e8bf2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8bf2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e8bf2-112">notConfigured</span></span>|<span data-ttu-id="e8bf2-113">0</span><span class="sxs-lookup"><span data-stu-id="e8bf2-113">0</span></span>|<span data-ttu-id="e8bf2-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="e8bf2-114">Not Configured</span></span>|
|<span data-ttu-id="e8bf2-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="e8bf2-115">blockBoth</span></span>|<span data-ttu-id="e8bf2-116">1</span><span class="sxs-lookup"><span data-stu-id="e8bf2-116">1</span></span>|<span data-ttu-id="e8bf2-117">ブロックのクリップボード データのコンテナーにホストとホスト コンテナーの両方を共有するには</span><span class="sxs-lookup"><span data-stu-id="e8bf2-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="e8bf2-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="e8bf2-118">blockHostToContainer</span></span>|<span data-ttu-id="e8bf2-119">2</span><span class="sxs-lookup"><span data-stu-id="e8bf2-119">2</span></span>|<span data-ttu-id="e8bf2-120">コンテナーにホストからのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="e8bf2-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="e8bf2-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="e8bf2-121">blockContainerToHost</span></span>|<span data-ttu-id="e8bf2-122">3</span><span class="sxs-lookup"><span data-stu-id="e8bf2-122">3</span></span>|<span data-ttu-id="e8bf2-123">コンテナーからホストへのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="e8bf2-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="e8bf2-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="e8bf2-124">blockNone</span></span>|<span data-ttu-id="e8bf2-125">4</span><span class="sxs-lookup"><span data-stu-id="e8bf2-125">4</span></span>|<span data-ttu-id="e8bf2-126">ブロックのクリップボード データのコンテナーにホストもホストするためのコンテナーを共有するには</span><span class="sxs-lookup"><span data-stu-id="e8bf2-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





