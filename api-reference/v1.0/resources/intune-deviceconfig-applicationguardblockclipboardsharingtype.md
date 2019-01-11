---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6fe418aa1f91c0e65770b797781dda9e29803d86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865976"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="77fd4-103">applicationGuardBlockClipboardSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="77fd4-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="77fd4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="77fd4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77fd4-105">ApplicationGuardBlockClipboardSharingType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="77fd4-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="77fd4-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="77fd4-106">Members</span></span>
|<span data-ttu-id="77fd4-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="77fd4-107">Member</span></span>|<span data-ttu-id="77fd4-108">値</span><span class="sxs-lookup"><span data-stu-id="77fd4-108">Value</span></span>|<span data-ttu-id="77fd4-109">説明</span><span class="sxs-lookup"><span data-stu-id="77fd4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77fd4-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="77fd4-110">notConfigured</span></span>|<span data-ttu-id="77fd4-111">0</span><span class="sxs-lookup"><span data-stu-id="77fd4-111">0</span></span>|<span data-ttu-id="77fd4-112">構成されていません</span><span class="sxs-lookup"><span data-stu-id="77fd4-112">Not Configured</span></span>|
|<span data-ttu-id="77fd4-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="77fd4-113">blockBoth</span></span>|<span data-ttu-id="77fd4-114">1</span><span class="sxs-lookup"><span data-stu-id="77fd4-114">1</span></span>|<span data-ttu-id="77fd4-115">ブロックのクリップボード データのコンテナーにホストとホスト コンテナーの両方を共有するには</span><span class="sxs-lookup"><span data-stu-id="77fd4-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="77fd4-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="77fd4-116">blockHostToContainer</span></span>|<span data-ttu-id="77fd4-117">2</span><span class="sxs-lookup"><span data-stu-id="77fd4-117">2</span></span>|<span data-ttu-id="77fd4-118">コンテナーにホストからのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="77fd4-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="77fd4-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="77fd4-119">blockContainerToHost</span></span>|<span data-ttu-id="77fd4-120">3</span><span class="sxs-lookup"><span data-stu-id="77fd4-120">3</span></span>|<span data-ttu-id="77fd4-121">コンテナーからホストへのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="77fd4-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="77fd4-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="77fd4-122">blockNone</span></span>|<span data-ttu-id="77fd4-123">4</span><span class="sxs-lookup"><span data-stu-id="77fd4-123">4</span></span>|<span data-ttu-id="77fd4-124">ブロックのクリップボード データのコンテナーにホストもホストするためのコンテナーを共有するには</span><span class="sxs-lookup"><span data-stu-id="77fd4-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



