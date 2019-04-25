---
title: applicationgu/blockクリップの sharingtype 列挙型
description: applicationgu/blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d1b5132773bb0bf92f35c39b660726d7a1ef66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575080"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="871b0-103">applicationgu/blockクリップの sharingtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="871b0-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="871b0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="871b0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="871b0-105">applicationgu/blockblocksharingsharingtype に指定できる値</span><span class="sxs-lookup"><span data-stu-id="871b0-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="871b0-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="871b0-106">Members</span></span>
|<span data-ttu-id="871b0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="871b0-107">Member</span></span>|<span data-ttu-id="871b0-108">値</span><span class="sxs-lookup"><span data-stu-id="871b0-108">Value</span></span>|<span data-ttu-id="871b0-109">説明</span><span class="sxs-lookup"><span data-stu-id="871b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="871b0-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="871b0-110">notConfigured</span></span>|<span data-ttu-id="871b0-111">.0</span><span class="sxs-lookup"><span data-stu-id="871b0-111">0</span></span>|<span data-ttu-id="871b0-112">Not Configured</span><span class="sxs-lookup"><span data-stu-id="871b0-112">Not Configured</span></span>|
|<span data-ttu-id="871b0-113">blockboth</span><span class="sxs-lookup"><span data-stu-id="871b0-113">blockBoth</span></span>|<span data-ttu-id="871b0-114">1 </span><span class="sxs-lookup"><span data-stu-id="871b0-114">1</span></span>|<span data-ttu-id="871b0-115">ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード</span><span class="sxs-lookup"><span data-stu-id="871b0-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="871b0-116">blockhosttocontainer</span><span class="sxs-lookup"><span data-stu-id="871b0-116">blockHostToContainer</span></span>|<span data-ttu-id="871b0-117">2 </span><span class="sxs-lookup"><span data-stu-id="871b0-117">2</span></span>|<span data-ttu-id="871b0-118">データをホストからコンテナーに共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="871b0-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="871b0-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="871b0-119">blockContainerToHost</span></span>|<span data-ttu-id="871b0-120">3 </span><span class="sxs-lookup"><span data-stu-id="871b0-120">3</span></span>|<span data-ttu-id="871b0-121">コンテナーからホストへのデータを共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="871b0-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="871b0-122">blocknone</span><span class="sxs-lookup"><span data-stu-id="871b0-122">blockNone</span></span>|<span data-ttu-id="871b0-123">4 </span><span class="sxs-lookup"><span data-stu-id="871b0-123">4</span></span>|<span data-ttu-id="871b0-124">データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="871b0-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



