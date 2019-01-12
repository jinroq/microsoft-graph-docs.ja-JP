---
title: applicationGuardBlockFileTransferType 列挙型
description: ApplicationGuardBlockFileTransfer に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f6eb5c7c3f26fb62e73e9b1e103d111f6c652f5c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931266"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="d5641-103">applicationGuardBlockFileTransferType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d5641-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="d5641-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5641-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5641-105">ApplicationGuardBlockFileTransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="d5641-105">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="d5641-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5641-106">Members</span></span>
|<span data-ttu-id="d5641-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5641-107">Member</span></span>|<span data-ttu-id="d5641-108">値</span><span class="sxs-lookup"><span data-stu-id="d5641-108">Value</span></span>|<span data-ttu-id="d5641-109">説明</span><span class="sxs-lookup"><span data-stu-id="d5641-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5641-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d5641-110">notConfigured</span></span>|<span data-ttu-id="d5641-111">0</span><span class="sxs-lookup"><span data-stu-id="d5641-111">0</span></span>|<span data-ttu-id="d5641-112">構成されていません</span><span class="sxs-lookup"><span data-stu-id="d5641-112">Not Configured</span></span>|
|<span data-ttu-id="d5641-113">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="d5641-113">blockImageAndTextFile</span></span>|<span data-ttu-id="d5641-114">1</span><span class="sxs-lookup"><span data-stu-id="d5641-114">1</span></span>|<span data-ttu-id="d5641-115">イメージおよびテキストのファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="d5641-115">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="d5641-116">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="d5641-116">blockImageFile</span></span>|<span data-ttu-id="d5641-117">2</span><span class="sxs-lookup"><span data-stu-id="d5641-117">2</span></span>|<span data-ttu-id="d5641-118">イメージ ファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="d5641-118">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="d5641-119">blockNone</span><span class="sxs-lookup"><span data-stu-id="d5641-119">blockNone</span></span>|<span data-ttu-id="d5641-120">3</span><span class="sxs-lookup"><span data-stu-id="d5641-120">3</span></span>|<span data-ttu-id="d5641-121">転送がブロックされたテキスト ファイルまたはイメージ ファイルのどちらでもないです。</span><span class="sxs-lookup"><span data-stu-id="d5641-121">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="d5641-122">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="d5641-122">blockTextFile</span></span>|<span data-ttu-id="d5641-123">4</span><span class="sxs-lookup"><span data-stu-id="d5641-123">4</span></span>|<span data-ttu-id="d5641-124">ブロックのクリップボードのテキスト ファイルを転送するには</span><span class="sxs-lookup"><span data-stu-id="d5641-124">Block clipboard to transfer Text file</span></span>|



