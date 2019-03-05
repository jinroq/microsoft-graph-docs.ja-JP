---
title: applicationgu/blockfiletransfertype 列挙型
description: applicationgu/blockfiletransfer に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ac7a72dc05250f7bf2aa8256647d34d96882e8e5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254535"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="d7266-103">applicationgu/blockfiletransfertype 列挙型</span><span class="sxs-lookup"><span data-stu-id="d7266-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="d7266-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d7266-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7266-105">applicationgu/blockfiletransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="d7266-105">Possible values for applicationGuardBlockFileTransfer</span></span>

## <a name="members"></a><span data-ttu-id="d7266-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d7266-106">Members</span></span>
|<span data-ttu-id="d7266-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d7266-107">Member</span></span>|<span data-ttu-id="d7266-108">値</span><span class="sxs-lookup"><span data-stu-id="d7266-108">Value</span></span>|<span data-ttu-id="d7266-109">説明</span><span class="sxs-lookup"><span data-stu-id="d7266-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7266-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d7266-110">notConfigured</span></span>|<span data-ttu-id="d7266-111">.0</span><span class="sxs-lookup"><span data-stu-id="d7266-111">0</span></span>|<span data-ttu-id="d7266-112">未構成</span><span class="sxs-lookup"><span data-stu-id="d7266-112">Not Configured</span></span>|
|<span data-ttu-id="d7266-113">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="d7266-113">blockImageAndTextFile</span></span>|<span data-ttu-id="d7266-114">1-d</span><span class="sxs-lookup"><span data-stu-id="d7266-114">1</span></span>|<span data-ttu-id="d7266-115">画像とテキストファイルを転送するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="d7266-115">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="d7266-116">blockimagefile</span><span class="sxs-lookup"><span data-stu-id="d7266-116">blockImageFile</span></span>|<span data-ttu-id="d7266-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d7266-117">2</span></span>|<span data-ttu-id="d7266-118">クリップボードをブロックしてイメージファイルを転送する</span><span class="sxs-lookup"><span data-stu-id="d7266-118">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="d7266-119">blocknone</span><span class="sxs-lookup"><span data-stu-id="d7266-119">blockNone</span></span>|<span data-ttu-id="d7266-120">1/3</span><span class="sxs-lookup"><span data-stu-id="d7266-120">3</span></span>|<span data-ttu-id="d7266-121">テキストファイルまたはイメージファイルの転送がブロックされません</span><span class="sxs-lookup"><span data-stu-id="d7266-121">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="d7266-122">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="d7266-122">blockTextFile</span></span>|<span data-ttu-id="d7266-123">2/4</span><span class="sxs-lookup"><span data-stu-id="d7266-123">4</span></span>|<span data-ttu-id="d7266-124">クリップボードからテキストファイルへの転送をブロックする</span><span class="sxs-lookup"><span data-stu-id="d7266-124">Block clipboard to transfer Text file</span></span>|



