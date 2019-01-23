---
title: applicationGuardBlockFileTransferType 列挙型
description: ApplicationGuardBlockFileTransfer に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9997956d192686a5287e181b25bd5f98184299c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396274"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="8a18c-103">applicationGuardBlockFileTransferType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8a18c-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="8a18c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a18c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8a18c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a18c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a18c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a18c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a18c-107">ApplicationGuardBlockFileTransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="8a18c-107">Possible values for applicationGuardBlockFileTransfer</span></span>

## <a name="members"></a><span data-ttu-id="8a18c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a18c-108">Members</span></span>
|<span data-ttu-id="8a18c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8a18c-109">Member</span></span>|<span data-ttu-id="8a18c-110">値</span><span class="sxs-lookup"><span data-stu-id="8a18c-110">Value</span></span>|<span data-ttu-id="8a18c-111">説明</span><span class="sxs-lookup"><span data-stu-id="8a18c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a18c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8a18c-112">notConfigured</span></span>|<span data-ttu-id="8a18c-113">0</span><span class="sxs-lookup"><span data-stu-id="8a18c-113">0</span></span>|<span data-ttu-id="8a18c-114">構成されていません</span><span class="sxs-lookup"><span data-stu-id="8a18c-114">Not Configured</span></span>|
|<span data-ttu-id="8a18c-115">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="8a18c-115">blockImageAndTextFile</span></span>|<span data-ttu-id="8a18c-116">1</span><span class="sxs-lookup"><span data-stu-id="8a18c-116">1</span></span>|<span data-ttu-id="8a18c-117">イメージおよびテキストのファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="8a18c-117">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="8a18c-118">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="8a18c-118">blockImageFile</span></span>|<span data-ttu-id="8a18c-119">2</span><span class="sxs-lookup"><span data-stu-id="8a18c-119">2</span></span>|<span data-ttu-id="8a18c-120">イメージ ファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="8a18c-120">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="8a18c-121">blockNone</span><span class="sxs-lookup"><span data-stu-id="8a18c-121">blockNone</span></span>|<span data-ttu-id="8a18c-122">3</span><span class="sxs-lookup"><span data-stu-id="8a18c-122">3</span></span>|<span data-ttu-id="8a18c-123">転送がブロックされたテキスト ファイルまたはイメージ ファイルのどちらでもないです。</span><span class="sxs-lookup"><span data-stu-id="8a18c-123">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="8a18c-124">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="8a18c-124">blockTextFile</span></span>|<span data-ttu-id="8a18c-125">4</span><span class="sxs-lookup"><span data-stu-id="8a18c-125">4</span></span>|<span data-ttu-id="8a18c-126">ブロックのクリップボードのテキスト ファイルを転送するには</span><span class="sxs-lookup"><span data-stu-id="8a18c-126">Block clipboard to transfer Text file</span></span>|




