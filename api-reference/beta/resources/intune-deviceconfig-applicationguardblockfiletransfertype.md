---
title: Applicationgu/Blockfiletransfertype 列挙型
description: Applicationgu/Blockfiletransfer に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 14b626333ad275642774ac7fcfa1ad1d511b226d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333941"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="6e488-103">Applicationgu/Blockfiletransfertype 列挙型</span><span class="sxs-lookup"><span data-stu-id="6e488-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="6e488-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6e488-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e488-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6e488-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e488-106">Applicationgu/Blockfiletransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="6e488-106">Possible values for applicationGuardBlockFileTransfer</span></span>

## <a name="members"></a><span data-ttu-id="6e488-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6e488-107">Members</span></span>
|<span data-ttu-id="6e488-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6e488-108">Member</span></span>|<span data-ttu-id="6e488-109">値</span><span class="sxs-lookup"><span data-stu-id="6e488-109">Value</span></span>|<span data-ttu-id="6e488-110">説明</span><span class="sxs-lookup"><span data-stu-id="6e488-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e488-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6e488-111">notConfigured</span></span>|<span data-ttu-id="6e488-112">.0</span><span class="sxs-lookup"><span data-stu-id="6e488-112">0</span></span>|<span data-ttu-id="6e488-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="6e488-113">Not Configured</span></span>|
|<span data-ttu-id="6e488-114">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="6e488-114">blockImageAndTextFile</span></span>|<span data-ttu-id="6e488-115">1-d</span><span class="sxs-lookup"><span data-stu-id="6e488-115">1</span></span>|<span data-ttu-id="6e488-116">画像とテキストファイルを転送するためのクリップボードをブロックする</span><span class="sxs-lookup"><span data-stu-id="6e488-116">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="6e488-117">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="6e488-117">blockImageFile</span></span>|<span data-ttu-id="6e488-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6e488-118">2</span></span>|<span data-ttu-id="6e488-119">クリップボードをブロックしてイメージファイルを転送する</span><span class="sxs-lookup"><span data-stu-id="6e488-119">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="6e488-120">blockNone</span><span class="sxs-lookup"><span data-stu-id="6e488-120">blockNone</span></span>|<span data-ttu-id="6e488-121">1/3</span><span class="sxs-lookup"><span data-stu-id="6e488-121">3</span></span>|<span data-ttu-id="6e488-122">テキストファイルまたはイメージファイルの転送がブロックされません</span><span class="sxs-lookup"><span data-stu-id="6e488-122">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="6e488-123">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="6e488-123">blockTextFile</span></span>|<span data-ttu-id="6e488-124">2/4</span><span class="sxs-lookup"><span data-stu-id="6e488-124">4</span></span>|<span data-ttu-id="6e488-125">クリップボードからテキストファイルへの転送をブロックする</span><span class="sxs-lookup"><span data-stu-id="6e488-125">Block clipboard to transfer Text file</span></span>|



