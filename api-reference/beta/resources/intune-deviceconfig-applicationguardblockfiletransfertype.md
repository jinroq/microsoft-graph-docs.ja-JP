---
title: applicationgu/blockfiletransfertype 列挙型
description: applicationgu/blockfiletransfer に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32b2d4ef3aabf8082074215825c8e3e08a44ba63
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142317"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="d7dea-103">applicationgu/blockfiletransfertype 列挙型</span><span class="sxs-lookup"><span data-stu-id="d7dea-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="d7dea-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7dea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7dea-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7dea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7dea-106">applicationgu/blockfiletransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="d7dea-106">Possible values for applicationGuardBlockFileTransfer</span></span>

## <a name="members"></a><span data-ttu-id="d7dea-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d7dea-107">Members</span></span>
|<span data-ttu-id="d7dea-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d7dea-108">Member</span></span>|<span data-ttu-id="d7dea-109">値</span><span class="sxs-lookup"><span data-stu-id="d7dea-109">Value</span></span>|<span data-ttu-id="d7dea-110">説明</span><span class="sxs-lookup"><span data-stu-id="d7dea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7dea-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d7dea-111">notConfigured</span></span>|<span data-ttu-id="d7dea-112">.0</span><span class="sxs-lookup"><span data-stu-id="d7dea-112">0</span></span>|<span data-ttu-id="d7dea-113">未構成</span><span class="sxs-lookup"><span data-stu-id="d7dea-113">Not Configured</span></span>|
|<span data-ttu-id="d7dea-114">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="d7dea-114">blockImageAndTextFile</span></span>|<span data-ttu-id="d7dea-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d7dea-115">1</span></span>|<span data-ttu-id="d7dea-116">画像とテキストファイルを転送するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="d7dea-116">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="d7dea-117">blockimagefile</span><span class="sxs-lookup"><span data-stu-id="d7dea-117">blockImageFile</span></span>|<span data-ttu-id="d7dea-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d7dea-118">2</span></span>|<span data-ttu-id="d7dea-119">クリップボードをブロックしてイメージファイルを転送する</span><span class="sxs-lookup"><span data-stu-id="d7dea-119">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="d7dea-120">blocknone</span><span class="sxs-lookup"><span data-stu-id="d7dea-120">blockNone</span></span>|<span data-ttu-id="d7dea-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d7dea-121">3</span></span>|<span data-ttu-id="d7dea-122">テキストファイルまたはイメージファイルの転送がブロックされません</span><span class="sxs-lookup"><span data-stu-id="d7dea-122">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="d7dea-123">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="d7dea-123">blockTextFile</span></span>|<span data-ttu-id="d7dea-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d7dea-124">4</span></span>|<span data-ttu-id="d7dea-125">クリップボードからテキストファイルへの転送をブロックする</span><span class="sxs-lookup"><span data-stu-id="d7dea-125">Block clipboard to transfer Text file</span></span>|




