---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f9621db53e16231f710cccb12d79f65d22d4017
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415062"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="c97f9-103">applicationGuardBlockClipboardSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c97f9-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="c97f9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c97f9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c97f9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c97f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c97f9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c97f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c97f9-107">ApplicationGuardBlockClipboardSharingType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="c97f9-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="c97f9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c97f9-108">Members</span></span>
|<span data-ttu-id="c97f9-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c97f9-109">Member</span></span>|<span data-ttu-id="c97f9-110">値</span><span class="sxs-lookup"><span data-stu-id="c97f9-110">Value</span></span>|<span data-ttu-id="c97f9-111">説明</span><span class="sxs-lookup"><span data-stu-id="c97f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c97f9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c97f9-112">notConfigured</span></span>|<span data-ttu-id="c97f9-113">0</span><span class="sxs-lookup"><span data-stu-id="c97f9-113">0</span></span>|<span data-ttu-id="c97f9-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="c97f9-114">Not Configured</span></span>|
|<span data-ttu-id="c97f9-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="c97f9-115">blockBoth</span></span>|<span data-ttu-id="c97f9-116">1</span><span class="sxs-lookup"><span data-stu-id="c97f9-116">1</span></span>|<span data-ttu-id="c97f9-117">ブロックのクリップボード データのコンテナーにホストとホスト コンテナーの両方を共有するには</span><span class="sxs-lookup"><span data-stu-id="c97f9-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="c97f9-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="c97f9-118">blockHostToContainer</span></span>|<span data-ttu-id="c97f9-119">2</span><span class="sxs-lookup"><span data-stu-id="c97f9-119">2</span></span>|<span data-ttu-id="c97f9-120">コンテナーにホストからのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="c97f9-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="c97f9-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="c97f9-121">blockContainerToHost</span></span>|<span data-ttu-id="c97f9-122">3</span><span class="sxs-lookup"><span data-stu-id="c97f9-122">3</span></span>|<span data-ttu-id="c97f9-123">コンテナーからホストへのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="c97f9-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="c97f9-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="c97f9-124">blockNone</span></span>|<span data-ttu-id="c97f9-125">4</span><span class="sxs-lookup"><span data-stu-id="c97f9-125">4</span></span>|<span data-ttu-id="c97f9-126">ブロックのクリップボード データのコンテナーにホストもホストするためのコンテナーを共有するには</span><span class="sxs-lookup"><span data-stu-id="c97f9-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




