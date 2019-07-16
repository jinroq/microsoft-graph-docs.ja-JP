---
title: Userpfxps/スキーム列挙型
description: 暗号化プロバイダーで使用される埋め込み方式のサポートされている値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a079075d3e0a44a773c854df55df1635d54584c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739275"
---
# <a name="userpfxpaddingscheme-enum-type"></a><span data-ttu-id="c15f3-103">Userpfxps/スキーム列挙型</span><span class="sxs-lookup"><span data-stu-id="c15f3-103">userPfxPaddingScheme enum type</span></span>

> <span data-ttu-id="c15f3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c15f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c15f3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c15f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c15f3-106">暗号化プロバイダーで使用される埋め込み方式のサポートされている値。</span><span class="sxs-lookup"><span data-stu-id="c15f3-106">Supported values for the padding scheme used by encryption provider.</span></span>

## <a name="members"></a><span data-ttu-id="c15f3-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c15f3-107">Members</span></span>
|<span data-ttu-id="c15f3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c15f3-108">Member</span></span>|<span data-ttu-id="c15f3-109">値</span><span class="sxs-lookup"><span data-stu-id="c15f3-109">Value</span></span>|<span data-ttu-id="c15f3-110">説明</span><span class="sxs-lookup"><span data-stu-id="c15f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c15f3-111">none</span><span class="sxs-lookup"><span data-stu-id="c15f3-111">none</span></span>|<span data-ttu-id="c15f3-112">.0</span><span class="sxs-lookup"><span data-stu-id="c15f3-112">0</span></span>|<span data-ttu-id="c15f3-113">パディングを使用しません。</span><span class="sxs-lookup"><span data-stu-id="c15f3-113">No padding used.</span></span>|
|<span data-ttu-id="c15f3-114">pkcs1</span><span class="sxs-lookup"><span data-stu-id="c15f3-114">pkcs1</span></span>|<span data-ttu-id="c15f3-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c15f3-115">1</span></span>|<span data-ttu-id="c15f3-116">PKCS # 1 のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="c15f3-116">Use PKCS#1 padding.</span></span>|
|<span data-ttu-id="c15f3-117">oaepSha1</span><span class="sxs-lookup"><span data-stu-id="c15f3-117">oaepSha1</span></span>|<span data-ttu-id="c15f3-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c15f3-118">2</span></span>|<span data-ttu-id="c15f3-119">OAEP のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="c15f3-119">Use OAEP SHA-1 padding.</span></span>|
|<span data-ttu-id="c15f3-120">oaepSha256</span><span class="sxs-lookup"><span data-stu-id="c15f3-120">oaepSha256</span></span>|<span data-ttu-id="c15f3-121">1/3</span><span class="sxs-lookup"><span data-stu-id="c15f3-121">3</span></span>|<span data-ttu-id="c15f3-122">OAEP 256 のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="c15f3-122">Use OAEP SHA-256 padding.</span></span>|
|<span data-ttu-id="c15f3-123">oaepSha384</span><span class="sxs-lookup"><span data-stu-id="c15f3-123">oaepSha384</span></span>|<span data-ttu-id="c15f3-124">2/4</span><span class="sxs-lookup"><span data-stu-id="c15f3-124">4</span></span>|<span data-ttu-id="c15f3-125">OAEP 384 のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="c15f3-125">Use OAEP SHA-384 padding.</span></span>|
|<span data-ttu-id="c15f3-126">oaepSha512</span><span class="sxs-lookup"><span data-stu-id="c15f3-126">oaepSha512</span></span>|<span data-ttu-id="c15f3-127">5</span><span class="sxs-lookup"><span data-stu-id="c15f3-127">5</span></span>|<span data-ttu-id="c15f3-128">OAEP 512 のパディングを使用します。</span><span class="sxs-lookup"><span data-stu-id="c15f3-128">Use OAEP SHA-512 padding.</span></span>|





