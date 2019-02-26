---
title: applicationgu/blockクリップの sharingtype 列挙型
description: applicationgu/blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d1b5132773bb0bf92f35c39b660726d7a1ef66
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261860"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="cd371-103">applicationgu/blockクリップの sharingtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="cd371-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="cd371-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cd371-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd371-105">applicationgu/blockblocksharingsharingtype に指定できる値</span><span class="sxs-lookup"><span data-stu-id="cd371-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="cd371-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="cd371-106">Members</span></span>
|<span data-ttu-id="cd371-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="cd371-107">Member</span></span>|<span data-ttu-id="cd371-108">値</span><span class="sxs-lookup"><span data-stu-id="cd371-108">Value</span></span>|<span data-ttu-id="cd371-109">説明</span><span class="sxs-lookup"><span data-stu-id="cd371-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd371-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cd371-110">notConfigured</span></span>|<span data-ttu-id="cd371-111">.0</span><span class="sxs-lookup"><span data-stu-id="cd371-111">0</span></span>|<span data-ttu-id="cd371-112">未構成</span><span class="sxs-lookup"><span data-stu-id="cd371-112">Not Configured</span></span>|
|<span data-ttu-id="cd371-113">blockboth</span><span class="sxs-lookup"><span data-stu-id="cd371-113">blockBoth</span></span>|<span data-ttu-id="cd371-114">1-d</span><span class="sxs-lookup"><span data-stu-id="cd371-114">1</span></span>|<span data-ttu-id="cd371-115">ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード</span><span class="sxs-lookup"><span data-stu-id="cd371-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="cd371-116">blockhosttocontainer</span><span class="sxs-lookup"><span data-stu-id="cd371-116">blockHostToContainer</span></span>|<span data-ttu-id="cd371-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="cd371-117">2</span></span>|<span data-ttu-id="cd371-118">データをホストからコンテナーに共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="cd371-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="cd371-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="cd371-119">blockContainerToHost</span></span>|<span data-ttu-id="cd371-120">1/3</span><span class="sxs-lookup"><span data-stu-id="cd371-120">3</span></span>|<span data-ttu-id="cd371-121">コンテナーからホストへのデータを共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="cd371-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="cd371-122">blocknone</span><span class="sxs-lookup"><span data-stu-id="cd371-122">blockNone</span></span>|<span data-ttu-id="cd371-123">2/4</span><span class="sxs-lookup"><span data-stu-id="cd371-123">4</span></span>|<span data-ttu-id="cd371-124">データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="cd371-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



