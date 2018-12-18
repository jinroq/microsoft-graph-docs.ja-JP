---
title: applicationGuardBlockFileTransferType 列挙型
description: ApplicationGuardBlockFileTransfer に指定できる値
author: tfitzmac
ms.openlocfilehash: 5ec313ea62341734152382f3ff7852bf8bc051bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326622"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="07589-103">applicationGuardBlockFileTransferType 列挙型</span><span class="sxs-lookup"><span data-stu-id="07589-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="07589-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="07589-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07589-105">ApplicationGuardBlockFileTransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="07589-105">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="07589-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="07589-106">Members</span></span>
|<span data-ttu-id="07589-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="07589-107">Member</span></span>|<span data-ttu-id="07589-108">値</span><span class="sxs-lookup"><span data-stu-id="07589-108">Value</span></span>|<span data-ttu-id="07589-109">説明</span><span class="sxs-lookup"><span data-stu-id="07589-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07589-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="07589-110">notConfigured</span></span>|<span data-ttu-id="07589-111">0</span><span class="sxs-lookup"><span data-stu-id="07589-111">0</span></span>|<span data-ttu-id="07589-112">構成されていません</span><span class="sxs-lookup"><span data-stu-id="07589-112">Not Configured</span></span>|
|<span data-ttu-id="07589-113">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="07589-113">blockImageAndTextFile</span></span>|<span data-ttu-id="07589-114">1</span><span class="sxs-lookup"><span data-stu-id="07589-114">1</span></span>|<span data-ttu-id="07589-115">イメージおよびテキストのファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="07589-115">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="07589-116">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="07589-116">blockImageFile</span></span>|<span data-ttu-id="07589-117">2</span><span class="sxs-lookup"><span data-stu-id="07589-117">2</span></span>|<span data-ttu-id="07589-118">イメージ ファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="07589-118">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="07589-119">blockNone</span><span class="sxs-lookup"><span data-stu-id="07589-119">blockNone</span></span>|<span data-ttu-id="07589-120">3</span><span class="sxs-lookup"><span data-stu-id="07589-120">3</span></span>|<span data-ttu-id="07589-121">転送がブロックされたテキスト ファイルまたはイメージ ファイルのどちらでもないです。</span><span class="sxs-lookup"><span data-stu-id="07589-121">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="07589-122">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="07589-122">blockTextFile</span></span>|<span data-ttu-id="07589-123">4</span><span class="sxs-lookup"><span data-stu-id="07589-123">4</span></span>|<span data-ttu-id="07589-124">ブロックのクリップボードのテキスト ファイルを転送するには</span><span class="sxs-lookup"><span data-stu-id="07589-124">Block clipboard to transfer Text file</span></span>|



