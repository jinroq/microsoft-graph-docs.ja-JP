---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
ms.openlocfilehash: 59d325612430a184feaf7df655a4da660b65ea78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021529"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="d05f3-103">applicationGuardBlockClipboardSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d05f3-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="d05f3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d05f3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d05f3-105">ApplicationGuardBlockClipboardSharingType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="d05f3-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="d05f3-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d05f3-106">Members</span></span>
|<span data-ttu-id="d05f3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d05f3-107">Member</span></span>|<span data-ttu-id="d05f3-108">値</span><span class="sxs-lookup"><span data-stu-id="d05f3-108">Value</span></span>|<span data-ttu-id="d05f3-109">説明</span><span class="sxs-lookup"><span data-stu-id="d05f3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d05f3-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d05f3-110">notConfigured</span></span>|<span data-ttu-id="d05f3-111">0</span><span class="sxs-lookup"><span data-stu-id="d05f3-111">0</span></span>|<span data-ttu-id="d05f3-112">構成されていません</span><span class="sxs-lookup"><span data-stu-id="d05f3-112">Not Configured</span></span>|
|<span data-ttu-id="d05f3-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="d05f3-113">blockBoth</span></span>|<span data-ttu-id="d05f3-114">1</span><span class="sxs-lookup"><span data-stu-id="d05f3-114">1</span></span>|<span data-ttu-id="d05f3-115">ブロックのクリップボード データのコンテナーにホストとホスト コンテナーの両方を共有するには</span><span class="sxs-lookup"><span data-stu-id="d05f3-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="d05f3-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="d05f3-116">blockHostToContainer</span></span>|<span data-ttu-id="d05f3-117">2</span><span class="sxs-lookup"><span data-stu-id="d05f3-117">2</span></span>|<span data-ttu-id="d05f3-118">コンテナーにホストからのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="d05f3-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="d05f3-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="d05f3-119">blockContainerToHost</span></span>|<span data-ttu-id="d05f3-120">3</span><span class="sxs-lookup"><span data-stu-id="d05f3-120">3</span></span>|<span data-ttu-id="d05f3-121">コンテナーからホストへのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="d05f3-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="d05f3-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="d05f3-122">blockNone</span></span>|<span data-ttu-id="d05f3-123">4</span><span class="sxs-lookup"><span data-stu-id="d05f3-123">4</span></span>|<span data-ttu-id="d05f3-124">ブロックのクリップボード データのコンテナーにホストもホストするためのコンテナーを共有するには</span><span class="sxs-lookup"><span data-stu-id="d05f3-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



