---
title: applicationGuardBlockFileTransferType 列挙型
description: ApplicationGuardBlockFileTransfer に指定できる値
ms.openlocfilehash: ba0143a86dfd51f9a981e7ea4d399ac48e37d167
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020164"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="4514a-103">applicationGuardBlockFileTransferType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4514a-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="4514a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4514a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4514a-105">ApplicationGuardBlockFileTransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="4514a-105">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="4514a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="4514a-106">Members</span></span>
|<span data-ttu-id="4514a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4514a-107">Member</span></span>|<span data-ttu-id="4514a-108">値</span><span class="sxs-lookup"><span data-stu-id="4514a-108">Value</span></span>|<span data-ttu-id="4514a-109">説明</span><span class="sxs-lookup"><span data-stu-id="4514a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4514a-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4514a-110">notConfigured</span></span>|<span data-ttu-id="4514a-111">0</span><span class="sxs-lookup"><span data-stu-id="4514a-111">0</span></span>|<span data-ttu-id="4514a-112">構成されていません</span><span class="sxs-lookup"><span data-stu-id="4514a-112">Not Configured</span></span>|
|<span data-ttu-id="4514a-113">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="4514a-113">blockImageAndTextFile</span></span>|<span data-ttu-id="4514a-114">1</span><span class="sxs-lookup"><span data-stu-id="4514a-114">1</span></span>|<span data-ttu-id="4514a-115">イメージおよびテキストのファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="4514a-115">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="4514a-116">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="4514a-116">blockImageFile</span></span>|<span data-ttu-id="4514a-117">2</span><span class="sxs-lookup"><span data-stu-id="4514a-117">2</span></span>|<span data-ttu-id="4514a-118">イメージ ファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="4514a-118">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="4514a-119">blockNone</span><span class="sxs-lookup"><span data-stu-id="4514a-119">blockNone</span></span>|<span data-ttu-id="4514a-120">3</span><span class="sxs-lookup"><span data-stu-id="4514a-120">3</span></span>|<span data-ttu-id="4514a-121">転送がブロックされたテキスト ファイルまたはイメージ ファイルのどちらでもないです。</span><span class="sxs-lookup"><span data-stu-id="4514a-121">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="4514a-122">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="4514a-122">blockTextFile</span></span>|<span data-ttu-id="4514a-123">4</span><span class="sxs-lookup"><span data-stu-id="4514a-123">4</span></span>|<span data-ttu-id="4514a-124">ブロックのクリップボードのテキスト ファイルを転送するには</span><span class="sxs-lookup"><span data-stu-id="4514a-124">Block clipboard to transfer Text file</span></span>|



