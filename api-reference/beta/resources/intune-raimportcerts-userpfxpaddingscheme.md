---
title: Userpfxps/スキーム列挙型
description: 暗号化プロバイダーで使用される埋め込み方式のサポートされている値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a3c4d4d07a3891167838af6de7ea854883a5b1e5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967701"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="7fca9-103">Userpfxps/スキーム列挙型</span><span class="sxs-lookup"><span data-stu-id="7fca9-103">userPfxPaddingScheme enum type</span></span>

> <span data-ttu-id="7fca9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7fca9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7fca9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7fca9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7fca9-106">暗号化プロバイダーで使用される埋め込み方式のサポートされている値。</span><span class="sxs-lookup"><span data-stu-id="7fca9-106">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="7fca9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7fca9-107">Members</span></span>
|<span data-ttu-id="7fca9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7fca9-108">Member</span></span>|<span data-ttu-id="7fca9-109">値</span><span class="sxs-lookup"><span data-stu-id="7fca9-109">Value</span></span>|<span data-ttu-id="7fca9-110">説明</span><span class="sxs-lookup"><span data-stu-id="7fca9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fca9-111">none</span><span class="sxs-lookup"><span data-stu-id="7fca9-111">none</span></span>|<span data-ttu-id="7fca9-112">.0</span><span class="sxs-lookup"><span data-stu-id="7fca9-112">0</span></span>|<span data-ttu-id="7fca9-113">パディングを使用しません。</span><span class="sxs-lookup"><span data-stu-id="7fca9-113">No padding used.</span></span>|
|<span data-ttu-id="7fca9-114">pkcs1</span><span class="sxs-lookup"><span data-stu-id="7fca9-114">pkcs1</span></span>|<span data-ttu-id="7fca9-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7fca9-115">1</span></span>|<span data-ttu-id="7fca9-116">PKCS # 1 のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="7fca9-116">Use PKCS#1 padding.</span></span>|
|<span data-ttu-id="7fca9-117">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="7fca9-117">oaepSha1</span></span>|<span data-ttu-id="7fca9-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7fca9-118">2</span></span>|<span data-ttu-id="7fca9-119">OAEP のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="7fca9-119">Use OAEP SHA-1 padding.</span></span>|
|<span data-ttu-id="7fca9-120">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="7fca9-120">oaepSha256</span></span>|<span data-ttu-id="7fca9-121">1/3</span><span class="sxs-lookup"><span data-stu-id="7fca9-121">3</span></span>|<span data-ttu-id="7fca9-122">OAEP 256 のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="7fca9-122">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="7fca9-123">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="7fca9-123">oaepSha384</span></span>|<span data-ttu-id="7fca9-124">2/4</span><span class="sxs-lookup"><span data-stu-id="7fca9-124">4</span></span>|<span data-ttu-id="7fca9-125">OAEP 384 のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="7fca9-125">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="7fca9-126">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="7fca9-126">oaepSha512</span></span>|<span data-ttu-id="7fca9-127">5</span><span class="sxs-lookup"><span data-stu-id="7fca9-127">5</span></span>|<span data-ttu-id="7fca9-128">OAEP 512 のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="7fca9-128">Use OAEP SHA-512 padding.</span></span>|





