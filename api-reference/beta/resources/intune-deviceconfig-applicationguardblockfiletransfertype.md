---
title: Applicationgu/Blockfiletransfertype 列挙型
description: Applicationgu/Blockfiletransfer に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bc98b3e72b444ba3eaf4527db7b2cc8c7b7c519d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947618"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="3ce06-103">Applicationgu/Blockfiletransfertype 列挙型</span><span class="sxs-lookup"><span data-stu-id="3ce06-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="3ce06-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ce06-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ce06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ce06-106">Applicationgu/Blockfiletransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="3ce06-106">Possible values for applicationGuardBlockFileTransfer</span></span>

## <a name="members"></a><span data-ttu-id="3ce06-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3ce06-107">Members</span></span>
|<span data-ttu-id="3ce06-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3ce06-108">Member</span></span>|<span data-ttu-id="3ce06-109">値</span><span class="sxs-lookup"><span data-stu-id="3ce06-109">Value</span></span>|<span data-ttu-id="3ce06-110">説明</span><span class="sxs-lookup"><span data-stu-id="3ce06-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ce06-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3ce06-111">notConfigured</span></span>|<span data-ttu-id="3ce06-112">.0</span><span class="sxs-lookup"><span data-stu-id="3ce06-112">0</span></span>|<span data-ttu-id="3ce06-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="3ce06-113">Not Configured</span></span>|
|<span data-ttu-id="3ce06-114">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="3ce06-114">blockImageAndTextFile</span></span>|<span data-ttu-id="3ce06-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3ce06-115">1</span></span>|<span data-ttu-id="3ce06-116">画像とテキストファイルを転送するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="3ce06-116">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="3ce06-117">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="3ce06-117">blockImageFile</span></span>|<span data-ttu-id="3ce06-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3ce06-118">2</span></span>|<span data-ttu-id="3ce06-119">クリップボードをブロックしてイメージファイルを転送する</span><span class="sxs-lookup"><span data-stu-id="3ce06-119">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="3ce06-120">blockNone</span><span class="sxs-lookup"><span data-stu-id="3ce06-120">blockNone</span></span>|<span data-ttu-id="3ce06-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3ce06-121">3</span></span>|<span data-ttu-id="3ce06-122">テキストファイルまたはイメージファイルの転送がブロックされません</span><span class="sxs-lookup"><span data-stu-id="3ce06-122">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="3ce06-123">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="3ce06-123">blockTextFile</span></span>|<span data-ttu-id="3ce06-124">2/4</span><span class="sxs-lookup"><span data-stu-id="3ce06-124">4</span></span>|<span data-ttu-id="3ce06-125">クリップボードからテキストファイルへの転送をブロックする</span><span class="sxs-lookup"><span data-stu-id="3ce06-125">Block clipboard to transfer Text file</span></span>|




