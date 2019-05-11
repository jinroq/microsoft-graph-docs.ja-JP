---
title: Applicationgu/Blockクリップの Sharingtype 列挙型
description: Applicationgu/Blockblocksharingsharingtype に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b5befd2a1967081c0be617d9438946875e41a9f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947744"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="f9172-103">Applicationgu/Blockクリップの Sharingtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="f9172-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="f9172-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9172-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9172-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9172-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9172-106">Applicationgu/Blockblocksharingsharingtype に指定できる値</span><span class="sxs-lookup"><span data-stu-id="f9172-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="f9172-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f9172-107">Members</span></span>
|<span data-ttu-id="f9172-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f9172-108">Member</span></span>|<span data-ttu-id="f9172-109">値</span><span class="sxs-lookup"><span data-stu-id="f9172-109">Value</span></span>|<span data-ttu-id="f9172-110">説明</span><span class="sxs-lookup"><span data-stu-id="f9172-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9172-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f9172-111">notConfigured</span></span>|<span data-ttu-id="f9172-112">.0</span><span class="sxs-lookup"><span data-stu-id="f9172-112">0</span></span>|<span data-ttu-id="f9172-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="f9172-113">Not Configured</span></span>|
|<span data-ttu-id="f9172-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="f9172-114">blockBoth</span></span>|<span data-ttu-id="f9172-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f9172-115">1</span></span>|<span data-ttu-id="f9172-116">ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード</span><span class="sxs-lookup"><span data-stu-id="f9172-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="f9172-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="f9172-117">blockHostToContainer</span></span>|<span data-ttu-id="f9172-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f9172-118">2</span></span>|<span data-ttu-id="f9172-119">データをホストからコンテナーに共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="f9172-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="f9172-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="f9172-120">blockContainerToHost</span></span>|<span data-ttu-id="f9172-121">1/3</span><span class="sxs-lookup"><span data-stu-id="f9172-121">3</span></span>|<span data-ttu-id="f9172-122">コンテナーからホストへのデータを共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="f9172-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="f9172-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="f9172-123">blockNone</span></span>|<span data-ttu-id="f9172-124">2/4</span><span class="sxs-lookup"><span data-stu-id="f9172-124">4</span></span>|<span data-ttu-id="f9172-125">データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="f9172-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




