---
title: applicationGuardBlockFileTransferType 列挙型
description: ApplicationGuardBlockFileTransfer に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 02eb1989c0218b66688f158461c4a66fa8c0a38a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871954"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="9fe42-103">applicationGuardBlockFileTransferType 列挙型</span><span class="sxs-lookup"><span data-stu-id="9fe42-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="9fe42-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9fe42-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fe42-105">ApplicationGuardBlockFileTransfer に指定できる値</span><span class="sxs-lookup"><span data-stu-id="9fe42-105">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="9fe42-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="9fe42-106">Members</span></span>
|<span data-ttu-id="9fe42-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9fe42-107">Member</span></span>|<span data-ttu-id="9fe42-108">値</span><span class="sxs-lookup"><span data-stu-id="9fe42-108">Value</span></span>|<span data-ttu-id="9fe42-109">説明</span><span class="sxs-lookup"><span data-stu-id="9fe42-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fe42-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9fe42-110">notConfigured</span></span>|<span data-ttu-id="9fe42-111">0</span><span class="sxs-lookup"><span data-stu-id="9fe42-111">0</span></span>|<span data-ttu-id="9fe42-112">構成されていません</span><span class="sxs-lookup"><span data-stu-id="9fe42-112">Not Configured</span></span>|
|<span data-ttu-id="9fe42-113">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="9fe42-113">blockImageAndTextFile</span></span>|<span data-ttu-id="9fe42-114">1</span><span class="sxs-lookup"><span data-stu-id="9fe42-114">1</span></span>|<span data-ttu-id="9fe42-115">イメージおよびテキストのファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="9fe42-115">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="9fe42-116">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="9fe42-116">blockImageFile</span></span>|<span data-ttu-id="9fe42-117">2</span><span class="sxs-lookup"><span data-stu-id="9fe42-117">2</span></span>|<span data-ttu-id="9fe42-118">イメージ ファイルを転送するブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="9fe42-118">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="9fe42-119">blockNone</span><span class="sxs-lookup"><span data-stu-id="9fe42-119">blockNone</span></span>|<span data-ttu-id="9fe42-120">3</span><span class="sxs-lookup"><span data-stu-id="9fe42-120">3</span></span>|<span data-ttu-id="9fe42-121">転送がブロックされたテキスト ファイルまたはイメージ ファイルのどちらでもないです。</span><span class="sxs-lookup"><span data-stu-id="9fe42-121">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="9fe42-122">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="9fe42-122">blockTextFile</span></span>|<span data-ttu-id="9fe42-123">4</span><span class="sxs-lookup"><span data-stu-id="9fe42-123">4</span></span>|<span data-ttu-id="9fe42-124">ブロックのクリップボードのテキスト ファイルを転送するには</span><span class="sxs-lookup"><span data-stu-id="9fe42-124">Block clipboard to transfer Text file</span></span>|



