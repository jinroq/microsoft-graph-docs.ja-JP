---
title: folderProtectionType 列挙型
description: フォルダー保護の可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3116e2663a9217e19f32f4e1c6cbc068d856fd0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994949"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="279ac-103">folderProtectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="279ac-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="279ac-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="279ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="279ac-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="279ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="279ac-106">フォルダー保護の可能な値</span><span class="sxs-lookup"><span data-stu-id="279ac-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="279ac-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="279ac-107">Members</span></span>
|<span data-ttu-id="279ac-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="279ac-108">Member</span></span>|<span data-ttu-id="279ac-109">値</span><span class="sxs-lookup"><span data-stu-id="279ac-109">Value</span></span>|<span data-ttu-id="279ac-110">説明</span><span class="sxs-lookup"><span data-stu-id="279ac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="279ac-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="279ac-111">userDefined</span></span>|<span data-ttu-id="279ac-112">.0</span><span class="sxs-lookup"><span data-stu-id="279ac-112">0</span></span>|<span data-ttu-id="279ac-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="279ac-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="279ac-114">使う</span><span class="sxs-lookup"><span data-stu-id="279ac-114">enable</span></span>|<span data-ttu-id="279ac-115">1-d</span><span class="sxs-lookup"><span data-stu-id="279ac-115">1</span></span>|<span data-ttu-id="279ac-116">機能をブロックする。</span><span class="sxs-lookup"><span data-stu-id="279ac-116">Block functionality.</span></span>|
|<span data-ttu-id="279ac-117">auditMode</span><span class="sxs-lookup"><span data-stu-id="279ac-117">auditMode</span></span>|<span data-ttu-id="279ac-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="279ac-118">2</span></span>|<span data-ttu-id="279ac-119">機能を有効にし、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="279ac-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="279ac-120">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="279ac-120">blockDiskModification</span></span>|<span data-ttu-id="279ac-121">1/3</span><span class="sxs-lookup"><span data-stu-id="279ac-121">3</span></span>|<span data-ttu-id="279ac-122">信頼されていないアプリのディスクセクターへの書き込みをブロックする。</span><span class="sxs-lookup"><span data-stu-id="279ac-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="279ac-123">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="279ac-123">auditDiskModification</span></span>|<span data-ttu-id="279ac-124">2/4</span><span class="sxs-lookup"><span data-stu-id="279ac-124">4</span></span>|<span data-ttu-id="279ac-125">信頼されていないアプリがディスクセクターに書き込むときにログを生成します。</span><span class="sxs-lookup"><span data-stu-id="279ac-125">Generate logs when untrusted apps write to disk sectors.</span></span>|





