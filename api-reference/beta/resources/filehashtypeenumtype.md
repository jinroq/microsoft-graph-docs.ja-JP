---
title: fileHashType 列挙型
description: ファイル ハッシュの種類を列挙します。
localization_priority: Normal
ms.openlocfilehash: e1c31aaea6c8cea40817efea61dc8654d3d17fae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816332"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="19593-103">fileHashType 列挙型</span><span class="sxs-lookup"><span data-stu-id="19593-103">fileHashType enum</span></span>

> <span data-ttu-id="19593-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19593-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19593-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19593-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19593-106">ファイル ハッシュの種類を列挙します。</span><span class="sxs-lookup"><span data-stu-id="19593-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="19593-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="19593-107">Members</span></span>

|<span data-ttu-id="19593-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="19593-108">Member</span></span>|<span data-ttu-id="19593-109">値</span><span class="sxs-lookup"><span data-stu-id="19593-109">Value</span></span>|<span data-ttu-id="19593-110">説明</span><span class="sxs-lookup"><span data-stu-id="19593-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19593-111">不明</span><span class="sxs-lookup"><span data-stu-id="19593-111">unknown</span></span>|<span data-ttu-id="19593-112">0</span><span class="sxs-lookup"><span data-stu-id="19593-112">0</span></span>|<span data-ttu-id="19593-113">不明な種類です。</span><span class="sxs-lookup"><span data-stu-id="19593-113">Unknown type.</span></span>|
|<span data-ttu-id="19593-114">sha1</span><span class="sxs-lookup"><span data-stu-id="19593-114">sha1</span></span>|<span data-ttu-id="19593-115">1</span><span class="sxs-lookup"><span data-stu-id="19593-115">1</span></span>|<span data-ttu-id="19593-116">SHA1 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="19593-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="19593-117">sha256</span><span class="sxs-lookup"><span data-stu-id="19593-117">sha256</span></span>|<span data-ttu-id="19593-118">2</span><span class="sxs-lookup"><span data-stu-id="19593-118">2</span></span>| <span data-ttu-id="19593-119">SHA256 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="19593-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="19593-120">md5</span><span class="sxs-lookup"><span data-stu-id="19593-120">md5</span></span>|<span data-ttu-id="19593-121">3</span><span class="sxs-lookup"><span data-stu-id="19593-121">3</span></span>| <span data-ttu-id="19593-122">MD5 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="19593-122">MD5 hash type.</span></span>|
|<span data-ttu-id="19593-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="19593-123">authenticodeHash256</span></span>|<span data-ttu-id="19593-124">4</span><span class="sxs-lookup"><span data-stu-id="19593-124">4</span></span>| <span data-ttu-id="19593-125">AuthenticodeHash256 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="19593-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="19593-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="19593-126">lsHash</span></span>|<span data-ttu-id="19593-127">5</span><span class="sxs-lookup"><span data-stu-id="19593-127">5</span></span>| <span data-ttu-id="19593-128">LsHash ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="19593-128">LsHash hash type.</span></span>|
|<span data-ttu-id="19593-129">ctph</span><span class="sxs-lookup"><span data-stu-id="19593-129">ctph</span></span>|<span data-ttu-id="19593-130">6</span><span class="sxs-lookup"><span data-stu-id="19593-130">6</span></span>| <span data-ttu-id="19593-131">CTPH ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="19593-131">CTPH hash type.</span></span>|
|<span data-ttu-id="19593-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="19593-132">peSha1</span></span>|<span data-ttu-id="19593-133">7</span><span class="sxs-lookup"><span data-stu-id="19593-133">7</span></span>| <span data-ttu-id="19593-134">PESHA1 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="19593-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="19593-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="19593-135">peSha256</span></span>|<span data-ttu-id="19593-136">8</span><span class="sxs-lookup"><span data-stu-id="19593-136">8</span></span>| <span data-ttu-id="19593-137">PESHA256 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="19593-137">PESHA256 hash type.</span></span>|
