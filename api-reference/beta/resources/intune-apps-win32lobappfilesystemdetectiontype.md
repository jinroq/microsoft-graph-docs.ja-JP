---
title: win32LobAppFileSystemDetectionType 列挙型
description: サポートされているすべてのファイルシステム検出の種類が含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08783d51d6d54b0ccf2cf6d7077185e9e1c286fb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804964"
---
# <a name="win32lobappfilesystemdetectiontype-enum-type"></a><span data-ttu-id="c4f0f-103">win32LobAppFileSystemDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c4f0f-103">win32LobAppFileSystemDetectionType enum type</span></span>

> <span data-ttu-id="c4f0f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4f0f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4f0f-106">サポートされているすべてのファイルシステム検出の種類が含まれます。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-106">Contains all supported file system detection type.</span></span>

## <a name="members"></a><span data-ttu-id="c4f0f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4f0f-107">Members</span></span>
|<span data-ttu-id="c4f0f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c4f0f-108">Member</span></span>|<span data-ttu-id="c4f0f-109">値</span><span class="sxs-lookup"><span data-stu-id="c4f0f-109">Value</span></span>|<span data-ttu-id="c4f0f-110">説明</span><span class="sxs-lookup"><span data-stu-id="c4f0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4f0f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c4f0f-111">notConfigured</span></span>|<span data-ttu-id="c4f0f-112">.0</span><span class="sxs-lookup"><span data-stu-id="c4f0f-112">0</span></span>|<span data-ttu-id="c4f0f-113">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-113">Not configured.</span></span>|
|<span data-ttu-id="c4f0f-114">ある</span><span class="sxs-lookup"><span data-stu-id="c4f0f-114">exists</span></span>|<span data-ttu-id="c4f0f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c4f0f-115">1</span></span>|<span data-ttu-id="c4f0f-116">指定したファイルまたはフォルダーが存在するかどうか。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-116">Whether the specified file or folder exists.</span></span>|
|<span data-ttu-id="c4f0f-117">modifiedDate</span><span class="sxs-lookup"><span data-stu-id="c4f0f-117">modifiedDate</span></span>|<span data-ttu-id="c4f0f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c4f0f-118">2</span></span>|<span data-ttu-id="c4f0f-119">最終変更日。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-119">Last modified date.</span></span>|
|<span data-ttu-id="c4f0f-120">createdDate</span><span class="sxs-lookup"><span data-stu-id="c4f0f-120">createdDate</span></span>|<span data-ttu-id="c4f0f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="c4f0f-121">3</span></span>|<span data-ttu-id="c4f0f-122">日付を作成しました。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-122">Created date.</span></span>|
|<span data-ttu-id="c4f0f-123">バージョン</span><span class="sxs-lookup"><span data-stu-id="c4f0f-123">version</span></span>|<span data-ttu-id="c4f0f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="c4f0f-124">4</span></span>|<span data-ttu-id="c4f0f-125">バージョン値の種類。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-125">Version value type.</span></span>|
|<span data-ttu-id="c4f0f-126">sizeinmb</span><span class="sxs-lookup"><span data-stu-id="c4f0f-126">sizeInMB</span></span>|<span data-ttu-id="c4f0f-127">5</span><span class="sxs-lookup"><span data-stu-id="c4f0f-127">5</span></span>|<span data-ttu-id="c4f0f-128">サイズ検出の種類。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-128">Size detection type.</span></span>|
|<span data-ttu-id="c4f0f-129">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="c4f0f-129">doesNotExist</span></span>|<span data-ttu-id="c4f0f-130">シックス</span><span class="sxs-lookup"><span data-stu-id="c4f0f-130">6</span></span>|<span data-ttu-id="c4f0f-131">指定したファイルまたはフォルダーが存在しません。</span><span class="sxs-lookup"><span data-stu-id="c4f0f-131">The specified file or folder does not exist.</span></span>|





