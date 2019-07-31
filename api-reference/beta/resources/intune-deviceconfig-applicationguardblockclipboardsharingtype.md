---
title: Applicationgu/Blockクリップの Sharingtype 列挙型
description: Applicationgu/Blockblocksharingsharingtype に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 09918437827524eeec00b819041a2fadb3705a10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004576"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="46328-103">Applicationgu/Blockクリップの Sharingtype 列挙型</span><span class="sxs-lookup"><span data-stu-id="46328-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="46328-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46328-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46328-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="46328-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46328-106">Applicationgu/Blockblocksharingsharingtype に指定できる値</span><span class="sxs-lookup"><span data-stu-id="46328-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="46328-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="46328-107">Members</span></span>
|<span data-ttu-id="46328-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="46328-108">Member</span></span>|<span data-ttu-id="46328-109">値</span><span class="sxs-lookup"><span data-stu-id="46328-109">Value</span></span>|<span data-ttu-id="46328-110">説明</span><span class="sxs-lookup"><span data-stu-id="46328-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46328-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="46328-111">notConfigured</span></span>|<span data-ttu-id="46328-112">.0</span><span class="sxs-lookup"><span data-stu-id="46328-112">0</span></span>|<span data-ttu-id="46328-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="46328-113">Not Configured</span></span>|
|<span data-ttu-id="46328-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="46328-114">blockBoth</span></span>|<span data-ttu-id="46328-115">1-d</span><span class="sxs-lookup"><span data-stu-id="46328-115">1</span></span>|<span data-ttu-id="46328-116">ホストからコンテナーへ、およびコンテナーからホストへのデータの共有をブロックするクリップボード</span><span class="sxs-lookup"><span data-stu-id="46328-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="46328-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="46328-117">blockHostToContainer</span></span>|<span data-ttu-id="46328-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="46328-118">2</span></span>|<span data-ttu-id="46328-119">データをホストからコンテナーに共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="46328-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="46328-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="46328-120">blockContainerToHost</span></span>|<span data-ttu-id="46328-121">1/3</span><span class="sxs-lookup"><span data-stu-id="46328-121">3</span></span>|<span data-ttu-id="46328-122">コンテナーからホストへのデータを共有するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="46328-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="46328-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="46328-123">blockNone</span></span>|<span data-ttu-id="46328-124">2/4</span><span class="sxs-lookup"><span data-stu-id="46328-124">4</span></span>|<span data-ttu-id="46328-125">データをホストからコンテナーにも、コンテナーからホストへも共有しないようにクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="46328-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





