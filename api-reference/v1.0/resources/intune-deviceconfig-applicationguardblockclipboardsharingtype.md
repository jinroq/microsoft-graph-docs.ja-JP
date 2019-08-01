---
title: Applicationgu/Blockクリップの Sharingtype 列挙型
description: Applicationgu/Blockblocksharingsharingtype に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a0c6263fe48876ed52e7da81b41975a781cc9636
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028645"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="b8ef7-103">Applicationgu/Blockクリップの Sharingtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="b8ef7-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="b8ef7-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8ef7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8ef7-105">Applicationgu/Blockblocksharingsharingtype に指定できる値</span><span class="sxs-lookup"><span data-stu-id="b8ef7-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="b8ef7-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="b8ef7-106">Members</span></span>
|<span data-ttu-id="b8ef7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b8ef7-107">Member</span></span>|<span data-ttu-id="b8ef7-108">値</span><span class="sxs-lookup"><span data-stu-id="b8ef7-108">Value</span></span>|<span data-ttu-id="b8ef7-109">説明</span><span class="sxs-lookup"><span data-stu-id="b8ef7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ef7-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b8ef7-110">notConfigured</span></span>|<span data-ttu-id="b8ef7-111">.0</span><span class="sxs-lookup"><span data-stu-id="b8ef7-111">0</span></span>|<span data-ttu-id="b8ef7-112">Not Configured</span><span class="sxs-lookup"><span data-stu-id="b8ef7-112">Not Configured</span></span>|
|<span data-ttu-id="b8ef7-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="b8ef7-113">blockBoth</span></span>|<span data-ttu-id="b8ef7-114">1-d</span><span class="sxs-lookup"><span data-stu-id="b8ef7-114">1</span></span>|<span data-ttu-id="b8ef7-115">ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード</span><span class="sxs-lookup"><span data-stu-id="b8ef7-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="b8ef7-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="b8ef7-116">blockHostToContainer</span></span>|<span data-ttu-id="b8ef7-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b8ef7-117">2</span></span>|<span data-ttu-id="b8ef7-118">データをホストからコンテナーに共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="b8ef7-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="b8ef7-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="b8ef7-119">blockContainerToHost</span></span>|<span data-ttu-id="b8ef7-120">1/3</span><span class="sxs-lookup"><span data-stu-id="b8ef7-120">3</span></span>|<span data-ttu-id="b8ef7-121">コンテナーからホストへのデータを共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="b8ef7-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="b8ef7-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="b8ef7-122">blockNone</span></span>|<span data-ttu-id="b8ef7-123">2/4</span><span class="sxs-lookup"><span data-stu-id="b8ef7-123">4</span></span>|<span data-ttu-id="b8ef7-124">データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="b8ef7-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



