---
title: folderProtectionType 列挙型
description: フォルダー保護の可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4cc114a1795cb68dd1f1a45a25e70b7128dea828
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946603"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="e6b20-103">folderProtectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e6b20-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="e6b20-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6b20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6b20-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e6b20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6b20-106">フォルダー保護の可能な値</span><span class="sxs-lookup"><span data-stu-id="e6b20-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="e6b20-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e6b20-107">Members</span></span>
|<span data-ttu-id="e6b20-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e6b20-108">Member</span></span>|<span data-ttu-id="e6b20-109">値</span><span class="sxs-lookup"><span data-stu-id="e6b20-109">Value</span></span>|<span data-ttu-id="e6b20-110">説明</span><span class="sxs-lookup"><span data-stu-id="e6b20-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6b20-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="e6b20-111">userDefined</span></span>|<span data-ttu-id="e6b20-112">.0</span><span class="sxs-lookup"><span data-stu-id="e6b20-112">0</span></span>|<span data-ttu-id="e6b20-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e6b20-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="e6b20-114">使う</span><span class="sxs-lookup"><span data-stu-id="e6b20-114">enable</span></span>|<span data-ttu-id="e6b20-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e6b20-115">1</span></span>|<span data-ttu-id="e6b20-116">機能をブロックする。</span><span class="sxs-lookup"><span data-stu-id="e6b20-116">Block functionality.</span></span>|
|<span data-ttu-id="e6b20-117">auditMode</span><span class="sxs-lookup"><span data-stu-id="e6b20-117">auditMode</span></span>|<span data-ttu-id="e6b20-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e6b20-118">2</span></span>|<span data-ttu-id="e6b20-119">機能を有効にし、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="e6b20-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="e6b20-120">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="e6b20-120">blockDiskModification</span></span>|<span data-ttu-id="e6b20-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e6b20-121">3</span></span>|<span data-ttu-id="e6b20-122">信頼されていないアプリのディスクセクターへの書き込みをブロックする。</span><span class="sxs-lookup"><span data-stu-id="e6b20-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="e6b20-123">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="e6b20-123">auditDiskModification</span></span>|<span data-ttu-id="e6b20-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e6b20-124">4</span></span>|<span data-ttu-id="e6b20-125">信頼されていないアプリがディスクセクターに書き込むときにログを生成します。</span><span class="sxs-lookup"><span data-stu-id="e6b20-125">Generate logs when untrusted apps write to disk sectors.</span></span>|




