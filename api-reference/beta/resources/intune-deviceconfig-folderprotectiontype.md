---
title: folderProtectionType 列挙型
description: フォルダーの保護の使用可能な値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2abbb719ab93b53ad276f8391d4028c4f8b40b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405717"
---
# <a name="folderprotectiontype-enum-type"></a><span data-ttu-id="8b608-103">folderProtectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="8b608-103">folderProtectionType enum type</span></span>

> <span data-ttu-id="8b608-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8b608-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8b608-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b608-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b608-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8b608-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b608-107">フォルダーの保護の使用可能な値</span><span class="sxs-lookup"><span data-stu-id="8b608-107">Possible values of Folder Protection</span></span>

## <a name="members"></a><span data-ttu-id="8b608-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8b608-108">Members</span></span>
|<span data-ttu-id="8b608-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8b608-109">Member</span></span>|<span data-ttu-id="8b608-110">値</span><span class="sxs-lookup"><span data-stu-id="8b608-110">Value</span></span>|<span data-ttu-id="8b608-111">説明</span><span class="sxs-lookup"><span data-stu-id="8b608-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b608-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="8b608-112">userDefined</span></span>|<span data-ttu-id="8b608-113">0</span><span class="sxs-lookup"><span data-stu-id="8b608-113">0</span></span>|<span data-ttu-id="8b608-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="8b608-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="8b608-115">有効にします。</span><span class="sxs-lookup"><span data-stu-id="8b608-115">enable</span></span>|<span data-ttu-id="8b608-116">1</span><span class="sxs-lookup"><span data-stu-id="8b608-116">1</span></span>|<span data-ttu-id="8b608-117">機能をブロックします。</span><span class="sxs-lookup"><span data-stu-id="8b608-117">Block functionality.</span></span>|
|<span data-ttu-id="8b608-118">auditMode</span><span class="sxs-lookup"><span data-stu-id="8b608-118">auditMode</span></span>|<span data-ttu-id="8b608-119">2</span><span class="sxs-lookup"><span data-stu-id="8b608-119">2</span></span>|<span data-ttu-id="8b608-120">機能を許可するが、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="8b608-120">Allow functionality but generate logs.</span></span>|
|<span data-ttu-id="8b608-121">blockDiskModification</span><span class="sxs-lookup"><span data-stu-id="8b608-121">blockDiskModification</span></span>|<span data-ttu-id="8b608-122">3</span><span class="sxs-lookup"><span data-stu-id="8b608-122">3</span></span>|<span data-ttu-id="8b608-123">ディスク ・ セクターへの書き込みから信頼されていないアプリケーションをブロックします。</span><span class="sxs-lookup"><span data-stu-id="8b608-123">Block untrusted apps from writing to disk sectors.</span></span>|
|<span data-ttu-id="8b608-124">auditDiskModification</span><span class="sxs-lookup"><span data-stu-id="8b608-124">auditDiskModification</span></span>|<span data-ttu-id="8b608-125">4</span><span class="sxs-lookup"><span data-stu-id="8b608-125">4</span></span>|<span data-ttu-id="8b608-126">信頼されていないアプリケーションがディスクのセクターに書き込むときは、ログを生成します。</span><span class="sxs-lookup"><span data-stu-id="8b608-126">Generate logs when untrusted apps write to disk sectors.</span></span>|




