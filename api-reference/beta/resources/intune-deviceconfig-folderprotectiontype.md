---
title: folderprotectiontype 列挙型
description: フォルダー保護の可能な値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0682f5bfbef65b982762e10a9425a8381d645d7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170337"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="83863-103">folderprotectiontype 列挙型</span><span class="sxs-lookup"><span data-stu-id="83863-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="83863-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83863-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83863-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83863-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83863-106">フォルダー保護の可能な値</span><span class="sxs-lookup"><span data-stu-id="83863-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="83863-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="83863-107">Members</span></span>
|<span data-ttu-id="83863-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="83863-108">Member</span></span>|<span data-ttu-id="83863-109">値</span><span class="sxs-lookup"><span data-stu-id="83863-109">Value</span></span>|<span data-ttu-id="83863-110">説明</span><span class="sxs-lookup"><span data-stu-id="83863-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83863-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="83863-111">userDefined</span></span>|<span data-ttu-id="83863-112">.0</span><span class="sxs-lookup"><span data-stu-id="83863-112">0</span></span>|<span data-ttu-id="83863-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="83863-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="83863-114">使う</span><span class="sxs-lookup"><span data-stu-id="83863-114">enable</span></span>|<span data-ttu-id="83863-115">1-d</span><span class="sxs-lookup"><span data-stu-id="83863-115">1</span></span>|<span data-ttu-id="83863-116">機能をブロックする。</span><span class="sxs-lookup"><span data-stu-id="83863-116">Block functionality.</span></span>|
|<span data-ttu-id="83863-117">auditmode</span><span class="sxs-lookup"><span data-stu-id="83863-117">auditMode</span></span>|<span data-ttu-id="83863-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="83863-118">2</span></span>|<span data-ttu-id="83863-119">機能を有効にし、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="83863-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="83863-120">blockdiskmodification</span><span class="sxs-lookup"><span data-stu-id="83863-120">blockDiskModification</span></span>|<span data-ttu-id="83863-121">1/3</span><span class="sxs-lookup"><span data-stu-id="83863-121">3</span></span>|<span data-ttu-id="83863-122">信頼されていないアプリのディスクセクターへの書き込みをブロックする。</span><span class="sxs-lookup"><span data-stu-id="83863-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="83863-123">auditdiskmodification</span><span class="sxs-lookup"><span data-stu-id="83863-123">auditDiskModification</span></span>|<span data-ttu-id="83863-124">2/4</span><span class="sxs-lookup"><span data-stu-id="83863-124">4</span></span>|<span data-ttu-id="83863-125">信頼されていないアプリがディスクセクターに書き込むときにログを生成します。</span><span class="sxs-lookup"><span data-stu-id="83863-125">Generate logs when untrusted apps write to disk sectors.</span></span>|




