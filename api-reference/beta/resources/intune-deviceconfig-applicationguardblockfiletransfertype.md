---
title: applicationGuardBlockFileTransferType 列挙型
description: ApplicationGuardBlockFileTransfer に指定できる値
author: tfitzmac
ms.openlocfilehash: fe1be9b0ceaee5651302b041b6612515557d899e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347391"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="53937-103">applicationGuardBlockFileTransferType 列挙型</span><span class="sxs-lookup"><span data-stu-id="53937-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="53937-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="53937-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53937-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53937-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53937-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="53937-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53937-107">ApplicationGuardBlockFileTransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="53937-107">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="53937-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="53937-108">Members</span></span>
|<span data-ttu-id="53937-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="53937-109">Member</span></span>|<span data-ttu-id="53937-110">値</span><span class="sxs-lookup"><span data-stu-id="53937-110">Value</span></span>|<span data-ttu-id="53937-111">説明</span><span class="sxs-lookup"><span data-stu-id="53937-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53937-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="53937-112">notConfigured</span></span>|<span data-ttu-id="53937-113">0</span><span class="sxs-lookup"><span data-stu-id="53937-113">0</span></span>|<span data-ttu-id="53937-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="53937-114">Not Configured</span></span>|
|<span data-ttu-id="53937-115">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="53937-115">blockImageAndTextFile</span></span>|<span data-ttu-id="53937-116">1</span><span class="sxs-lookup"><span data-stu-id="53937-116">1</span></span>|<span data-ttu-id="53937-117">イメージおよびテキストのファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="53937-117">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="53937-118">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="53937-118">blockImageFile</span></span>|<span data-ttu-id="53937-119">2</span><span class="sxs-lookup"><span data-stu-id="53937-119">2</span></span>|<span data-ttu-id="53937-120">イメージ ファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="53937-120">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="53937-121">blockNone</span><span class="sxs-lookup"><span data-stu-id="53937-121">blockNone</span></span>|<span data-ttu-id="53937-122">3</span><span class="sxs-lookup"><span data-stu-id="53937-122">3</span></span>|<span data-ttu-id="53937-123">転送がブロックされたテキスト ファイルまたはイメージ ファイルのどちらでもないです。</span><span class="sxs-lookup"><span data-stu-id="53937-123">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="53937-124">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="53937-124">blockTextFile</span></span>|<span data-ttu-id="53937-125">4</span><span class="sxs-lookup"><span data-stu-id="53937-125">4</span></span>|<span data-ttu-id="53937-126">ブロックのクリップボードのテキスト ファイルを転送するには</span><span class="sxs-lookup"><span data-stu-id="53937-126">Block clipboard to transfer Text file</span></span>|





