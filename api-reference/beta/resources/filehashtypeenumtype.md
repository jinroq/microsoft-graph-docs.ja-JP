---
title: fileHashType 列挙型
description: ファイル ハッシュの種類を列挙します。
ms.openlocfilehash: fbaa390ee8c543d2ed7c77cc05a11b519df0da9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067173"
---
# <a name="filehashtype-enum"></a><span data-ttu-id="52f5d-103">fileHashType 列挙型</span><span class="sxs-lookup"><span data-stu-id="52f5d-103">fileHashType enum</span></span>

> <span data-ttu-id="52f5d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="52f5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52f5d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52f5d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52f5d-106">ファイル ハッシュの種類を列挙します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-106">Enum for file hash types.</span></span>

## <a name="members"></a><span data-ttu-id="52f5d-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="52f5d-107">Members</span></span>

|<span data-ttu-id="52f5d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="52f5d-108">Member</span></span>|<span data-ttu-id="52f5d-109">値</span><span class="sxs-lookup"><span data-stu-id="52f5d-109">Value</span></span>|<span data-ttu-id="52f5d-110">説明</span><span class="sxs-lookup"><span data-stu-id="52f5d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52f5d-111">不明</span><span class="sxs-lookup"><span data-stu-id="52f5d-111">unknown</span></span>|<span data-ttu-id="52f5d-112">0</span><span class="sxs-lookup"><span data-stu-id="52f5d-112">0</span></span>|<span data-ttu-id="52f5d-113">不明な種類です。</span><span class="sxs-lookup"><span data-stu-id="52f5d-113">Unknown type.</span></span>|
|<span data-ttu-id="52f5d-114">sha1</span><span class="sxs-lookup"><span data-stu-id="52f5d-114">sha1</span></span>|<span data-ttu-id="52f5d-115">1</span><span class="sxs-lookup"><span data-stu-id="52f5d-115">1</span></span>|<span data-ttu-id="52f5d-116">SHA1 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-116">SHA1 hash type.</span></span>|
|<span data-ttu-id="52f5d-117">sha256</span><span class="sxs-lookup"><span data-stu-id="52f5d-117">sha256</span></span>|<span data-ttu-id="52f5d-118">2</span><span class="sxs-lookup"><span data-stu-id="52f5d-118">2</span></span>| <span data-ttu-id="52f5d-119">SHA256 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-119">SHA256 hash type.</span></span>|
|<span data-ttu-id="52f5d-120">md5</span><span class="sxs-lookup"><span data-stu-id="52f5d-120">md5</span></span>|<span data-ttu-id="52f5d-121">3</span><span class="sxs-lookup"><span data-stu-id="52f5d-121">3</span></span>| <span data-ttu-id="52f5d-122">MD5 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-122">MD5 hash type.</span></span>|
|<span data-ttu-id="52f5d-123">authenticodeHash256</span><span class="sxs-lookup"><span data-stu-id="52f5d-123">authenticodeHash256</span></span>|<span data-ttu-id="52f5d-124">4</span><span class="sxs-lookup"><span data-stu-id="52f5d-124">4</span></span>| <span data-ttu-id="52f5d-125">AuthenticodeHash256 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-125">AuthenticodeHash256 hash type.</span></span>|
|<span data-ttu-id="52f5d-126">lsHash</span><span class="sxs-lookup"><span data-stu-id="52f5d-126">lsHash</span></span>|<span data-ttu-id="52f5d-127">5</span><span class="sxs-lookup"><span data-stu-id="52f5d-127">5</span></span>| <span data-ttu-id="52f5d-128">LsHash ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-128">LsHash hash type.</span></span>|
|<span data-ttu-id="52f5d-129">ctph</span><span class="sxs-lookup"><span data-stu-id="52f5d-129">ctph</span></span>|<span data-ttu-id="52f5d-130">6</span><span class="sxs-lookup"><span data-stu-id="52f5d-130">6</span></span>| <span data-ttu-id="52f5d-131">CTPH ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-131">CTPH hash type.</span></span>|
|<span data-ttu-id="52f5d-132">peSha1</span><span class="sxs-lookup"><span data-stu-id="52f5d-132">peSha1</span></span>|<span data-ttu-id="52f5d-133">7</span><span class="sxs-lookup"><span data-stu-id="52f5d-133">7</span></span>| <span data-ttu-id="52f5d-134">PESHA1 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-134">PESHA1 hash type.</span></span>|
|<span data-ttu-id="52f5d-135">peSha256</span><span class="sxs-lookup"><span data-stu-id="52f5d-135">peSha256</span></span>|<span data-ttu-id="52f5d-136">8</span><span class="sxs-lookup"><span data-stu-id="52f5d-136">8</span></span>| <span data-ttu-id="52f5d-137">PESHA256 ハッシュ タイプを入力します。</span><span class="sxs-lookup"><span data-stu-id="52f5d-137">PESHA256 hash type.</span></span>|
