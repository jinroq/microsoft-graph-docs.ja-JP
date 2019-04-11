---
title: applicationgu/blockクリップの sharingtype 列挙型
description: applicationgu/blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83a0adf84ea57e6afa1749d1f6f7152403847b5f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806602"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="9c327-103">applicationgu/blockクリップの sharingtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="9c327-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="9c327-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c327-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c327-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9c327-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c327-106">applicationgu/blockblocksharingsharingtype に指定できる値</span><span class="sxs-lookup"><span data-stu-id="9c327-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="9c327-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9c327-107">Members</span></span>
|<span data-ttu-id="9c327-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9c327-108">Member</span></span>|<span data-ttu-id="9c327-109">値</span><span class="sxs-lookup"><span data-stu-id="9c327-109">Value</span></span>|<span data-ttu-id="9c327-110">説明</span><span class="sxs-lookup"><span data-stu-id="9c327-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c327-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9c327-111">notConfigured</span></span>|<span data-ttu-id="9c327-112">.0</span><span class="sxs-lookup"><span data-stu-id="9c327-112">0</span></span>|<span data-ttu-id="9c327-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="9c327-113">Not Configured</span></span>|
|<span data-ttu-id="9c327-114">blockboth</span><span class="sxs-lookup"><span data-stu-id="9c327-114">blockBoth</span></span>|<span data-ttu-id="9c327-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9c327-115">1</span></span>|<span data-ttu-id="9c327-116">ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード</span><span class="sxs-lookup"><span data-stu-id="9c327-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="9c327-117">blockhosttocontainer</span><span class="sxs-lookup"><span data-stu-id="9c327-117">blockHostToContainer</span></span>|<span data-ttu-id="9c327-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9c327-118">2</span></span>|<span data-ttu-id="9c327-119">データをホストからコンテナーに共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="9c327-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="9c327-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="9c327-120">blockContainerToHost</span></span>|<span data-ttu-id="9c327-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9c327-121">3</span></span>|<span data-ttu-id="9c327-122">コンテナーからホストへのデータを共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="9c327-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="9c327-123">blocknone</span><span class="sxs-lookup"><span data-stu-id="9c327-123">blockNone</span></span>|<span data-ttu-id="9c327-124">2/4</span><span class="sxs-lookup"><span data-stu-id="9c327-124">4</span></span>|<span data-ttu-id="9c327-125">データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="9c327-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





