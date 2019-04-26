---
title: applicationgu/blockfiletransfertype 列挙型
description: applicationgu/blockfiletransfer に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a35c830375195c9957884771b8e837a40ca984c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562294"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="2b0fd-103">applicationgu/blockfiletransfertype 列挙型</span><span class="sxs-lookup"><span data-stu-id="2b0fd-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="2b0fd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b0fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b0fd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2b0fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b0fd-106">applicationgu/blockfiletransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="2b0fd-106">Possible values for applicationGuardBlockFileTransfer</span></span>

## <a name="members"></a><span data-ttu-id="2b0fd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="2b0fd-107">Members</span></span>
|<span data-ttu-id="2b0fd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2b0fd-108">Member</span></span>|<span data-ttu-id="2b0fd-109">値</span><span class="sxs-lookup"><span data-stu-id="2b0fd-109">Value</span></span>|<span data-ttu-id="2b0fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="2b0fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b0fd-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2b0fd-111">notConfigured</span></span>|<span data-ttu-id="2b0fd-112">.0</span><span class="sxs-lookup"><span data-stu-id="2b0fd-112">0</span></span>|<span data-ttu-id="2b0fd-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="2b0fd-113">Not Configured</span></span>|
|<span data-ttu-id="2b0fd-114">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="2b0fd-114">blockImageAndTextFile</span></span>|<span data-ttu-id="2b0fd-115">1 </span><span class="sxs-lookup"><span data-stu-id="2b0fd-115">1</span></span>|<span data-ttu-id="2b0fd-116">画像とテキストファイルを転送するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="2b0fd-116">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="2b0fd-117">blockimagefile</span><span class="sxs-lookup"><span data-stu-id="2b0fd-117">blockImageFile</span></span>|<span data-ttu-id="2b0fd-118">2 </span><span class="sxs-lookup"><span data-stu-id="2b0fd-118">2</span></span>|<span data-ttu-id="2b0fd-119">クリップボードをブロックしてイメージファイルを転送する</span><span class="sxs-lookup"><span data-stu-id="2b0fd-119">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="2b0fd-120">blocknone</span><span class="sxs-lookup"><span data-stu-id="2b0fd-120">blockNone</span></span>|<span data-ttu-id="2b0fd-121">3 </span><span class="sxs-lookup"><span data-stu-id="2b0fd-121">3</span></span>|<span data-ttu-id="2b0fd-122">テキストファイルまたはイメージファイルの転送がブロックされません</span><span class="sxs-lookup"><span data-stu-id="2b0fd-122">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="2b0fd-123">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="2b0fd-123">blockTextFile</span></span>|<span data-ttu-id="2b0fd-124">4 </span><span class="sxs-lookup"><span data-stu-id="2b0fd-124">4</span></span>|<span data-ttu-id="2b0fd-125">クリップボードからテキストファイルへの転送をブロックする</span><span class="sxs-lookup"><span data-stu-id="2b0fd-125">Block clipboard to transfer Text file</span></span>|





