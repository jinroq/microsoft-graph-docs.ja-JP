---
title: applicationGuardBlockFileTransferType 列挙型
description: ApplicationGuardBlockFileTransfer に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 95da90b2b1210bb86032787b2fe26bc8a7c75391
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946729"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="58613-103">applicationGuardBlockFileTransferType 列挙型</span><span class="sxs-lookup"><span data-stu-id="58613-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="58613-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58613-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58613-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58613-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58613-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="58613-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58613-107">ApplicationGuardBlockFileTransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="58613-107">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="58613-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="58613-108">Members</span></span>
|<span data-ttu-id="58613-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="58613-109">Member</span></span>|<span data-ttu-id="58613-110">値</span><span class="sxs-lookup"><span data-stu-id="58613-110">Value</span></span>|<span data-ttu-id="58613-111">説明</span><span class="sxs-lookup"><span data-stu-id="58613-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58613-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="58613-112">notConfigured</span></span>|<span data-ttu-id="58613-113">0</span><span class="sxs-lookup"><span data-stu-id="58613-113">0</span></span>|<span data-ttu-id="58613-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="58613-114">Not Configured</span></span>|
|<span data-ttu-id="58613-115">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="58613-115">blockImageAndTextFile</span></span>|<span data-ttu-id="58613-116">1</span><span class="sxs-lookup"><span data-stu-id="58613-116">1</span></span>|<span data-ttu-id="58613-117">イメージおよびテキストのファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="58613-117">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="58613-118">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="58613-118">blockImageFile</span></span>|<span data-ttu-id="58613-119">2</span><span class="sxs-lookup"><span data-stu-id="58613-119">2</span></span>|<span data-ttu-id="58613-120">イメージ ファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="58613-120">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="58613-121">blockNone</span><span class="sxs-lookup"><span data-stu-id="58613-121">blockNone</span></span>|<span data-ttu-id="58613-122">3</span><span class="sxs-lookup"><span data-stu-id="58613-122">3</span></span>|<span data-ttu-id="58613-123">転送がブロックされたテキスト ファイルまたはイメージ ファイルのどちらでもないです。</span><span class="sxs-lookup"><span data-stu-id="58613-123">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="58613-124">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="58613-124">blockTextFile</span></span>|<span data-ttu-id="58613-125">4</span><span class="sxs-lookup"><span data-stu-id="58613-125">4</span></span>|<span data-ttu-id="58613-126">ブロックのクリップボードのテキスト ファイルを転送するには</span><span class="sxs-lookup"><span data-stu-id="58613-126">Block clipboard to transfer Text file</span></span>|





