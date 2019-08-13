---
title: folderProtectionType 列挙型
description: フォルダー保護の可能な値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8309fc7550252ebb3cc12ec05ca38e8bc611bb0f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338113"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="a5a5a-103">folderProtectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a5a5a-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="a5a5a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5a5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5a5a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5a5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5a5a-106">フォルダー保護の可能な値</span><span class="sxs-lookup"><span data-stu-id="a5a5a-106">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="a5a5a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a5a5a-107">Members</span></span>
|<span data-ttu-id="a5a5a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a5a5a-108">Member</span></span>|<span data-ttu-id="a5a5a-109">値</span><span class="sxs-lookup"><span data-stu-id="a5a5a-109">Value</span></span>|<span data-ttu-id="a5a5a-110">説明</span><span class="sxs-lookup"><span data-stu-id="a5a5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5a5a-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="a5a5a-111">userDefined</span></span>|<span data-ttu-id="a5a5a-112">.0</span><span class="sxs-lookup"><span data-stu-id="a5a5a-112">0</span></span>|<span data-ttu-id="a5a5a-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="a5a5a-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="a5a5a-114">使う</span><span class="sxs-lookup"><span data-stu-id="a5a5a-114">enable</span></span>|<span data-ttu-id="a5a5a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a5a5a-115">1</span></span>|<span data-ttu-id="a5a5a-116">機能をブロックする。</span><span class="sxs-lookup"><span data-stu-id="a5a5a-116">Block functionality.</span></span>|
|<span data-ttu-id="a5a5a-117">auditMode</span><span class="sxs-lookup"><span data-stu-id="a5a5a-117">auditMode</span></span>|<span data-ttu-id="a5a5a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a5a5a-118">2</span></span>|<span data-ttu-id="a5a5a-119">機能を有効にし、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="a5a5a-119">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="a5a5a-120">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="a5a5a-120">blockDiskModification</span></span>|<span data-ttu-id="a5a5a-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a5a5a-121">3</span></span>|<span data-ttu-id="a5a5a-122">信頼されていないアプリのディスクセクターへの書き込みをブロックする。</span><span class="sxs-lookup"><span data-stu-id="a5a5a-122">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="a5a5a-123">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="a5a5a-123">auditDiskModification</span></span>|<span data-ttu-id="a5a5a-124">2/4</span><span class="sxs-lookup"><span data-stu-id="a5a5a-124">4</span></span>|<span data-ttu-id="a5a5a-125">信頼されていないアプリがディスクセクターに書き込むときにログを生成します。</span><span class="sxs-lookup"><span data-stu-id="a5a5a-125">Generate logs when untrusted apps write to disk sectors.</span></span>|



