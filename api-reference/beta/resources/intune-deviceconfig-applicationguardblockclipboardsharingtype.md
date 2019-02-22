---
title: applicationgu/blockクリップの sharingtype 列挙型
description: applicationgu/blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dba5ba1a2d27862c9adaaa1430631b8cb4cf94d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160663"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="c01fd-103">applicationgu/blockクリップの sharingtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="c01fd-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="c01fd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c01fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c01fd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c01fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c01fd-106">applicationgu/blockblocksharingsharingtype に指定できる値</span><span class="sxs-lookup"><span data-stu-id="c01fd-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="c01fd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c01fd-107">Members</span></span>
|<span data-ttu-id="c01fd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c01fd-108">Member</span></span>|<span data-ttu-id="c01fd-109">値</span><span class="sxs-lookup"><span data-stu-id="c01fd-109">Value</span></span>|<span data-ttu-id="c01fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="c01fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c01fd-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c01fd-111">notConfigured</span></span>|<span data-ttu-id="c01fd-112">.0</span><span class="sxs-lookup"><span data-stu-id="c01fd-112">0</span></span>|<span data-ttu-id="c01fd-113">未構成</span><span class="sxs-lookup"><span data-stu-id="c01fd-113">Not Configured</span></span>|
|<span data-ttu-id="c01fd-114">blockboth</span><span class="sxs-lookup"><span data-stu-id="c01fd-114">blockBoth</span></span>|<span data-ttu-id="c01fd-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c01fd-115">1</span></span>|<span data-ttu-id="c01fd-116">ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード</span><span class="sxs-lookup"><span data-stu-id="c01fd-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="c01fd-117">blockhosttocontainer</span><span class="sxs-lookup"><span data-stu-id="c01fd-117">blockHostToContainer</span></span>|<span data-ttu-id="c01fd-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c01fd-118">2</span></span>|<span data-ttu-id="c01fd-119">データをホストからコンテナーに共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="c01fd-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="c01fd-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="c01fd-120">blockContainerToHost</span></span>|<span data-ttu-id="c01fd-121">1/3</span><span class="sxs-lookup"><span data-stu-id="c01fd-121">3</span></span>|<span data-ttu-id="c01fd-122">コンテナーからホストへのデータを共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="c01fd-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="c01fd-123">blocknone</span><span class="sxs-lookup"><span data-stu-id="c01fd-123">blockNone</span></span>|<span data-ttu-id="c01fd-124">2/4</span><span class="sxs-lookup"><span data-stu-id="c01fd-124">4</span></span>|<span data-ttu-id="c01fd-125">データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="c01fd-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




