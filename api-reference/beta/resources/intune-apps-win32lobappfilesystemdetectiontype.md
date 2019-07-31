---
title: win32LobAppFileSystemDetectionType 列挙型
description: サポートされているすべてのファイルシステム検出の種類が含まれます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e77e1a588946ca3a69a993fb561c1b48602602f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004975"
---
# <a name="win32lobappfilesystemdetectiontype-enum-type"></a><span data-ttu-id="08f5a-103">win32LobAppFileSystemDetectionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="08f5a-103">win32LobAppFileSystemDetectionType enum type</span></span>

> <span data-ttu-id="08f5a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08f5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08f5a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="08f5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08f5a-106">サポートされているすべてのファイルシステム検出の種類が含まれます。</span><span class="sxs-lookup"><span data-stu-id="08f5a-106">Contains all supported file system detection type.</span></span>

## <a name="members"></a><span data-ttu-id="08f5a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="08f5a-107">Members</span></span>
|<span data-ttu-id="08f5a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="08f5a-108">Member</span></span>|<span data-ttu-id="08f5a-109">値</span><span class="sxs-lookup"><span data-stu-id="08f5a-109">Value</span></span>|<span data-ttu-id="08f5a-110">説明</span><span class="sxs-lookup"><span data-stu-id="08f5a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08f5a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="08f5a-111">notConfigured</span></span>|<span data-ttu-id="08f5a-112">.0</span><span class="sxs-lookup"><span data-stu-id="08f5a-112">0</span></span>|<span data-ttu-id="08f5a-113">構成されていません。</span><span class="sxs-lookup"><span data-stu-id="08f5a-113">Not configured.</span></span>|
|<span data-ttu-id="08f5a-114">ある</span><span class="sxs-lookup"><span data-stu-id="08f5a-114">exists</span></span>|<span data-ttu-id="08f5a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="08f5a-115">1</span></span>|<span data-ttu-id="08f5a-116">指定したファイルまたはフォルダーが存在するかどうか。</span><span class="sxs-lookup"><span data-stu-id="08f5a-116">Whether the specified file or folder exists.</span></span>|
|<span data-ttu-id="08f5a-117">modifiedDate</span><span class="sxs-lookup"><span data-stu-id="08f5a-117">modifiedDate</span></span>|<span data-ttu-id="08f5a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="08f5a-118">2</span></span>|<span data-ttu-id="08f5a-119">最終変更日。</span><span class="sxs-lookup"><span data-stu-id="08f5a-119">Last modified date.</span></span>|
|<span data-ttu-id="08f5a-120">createdDate</span><span class="sxs-lookup"><span data-stu-id="08f5a-120">createdDate</span></span>|<span data-ttu-id="08f5a-121">1/3</span><span class="sxs-lookup"><span data-stu-id="08f5a-121">3</span></span>|<span data-ttu-id="08f5a-122">日付を作成しました。</span><span class="sxs-lookup"><span data-stu-id="08f5a-122">Created date.</span></span>|
|<span data-ttu-id="08f5a-123">バージョン</span><span class="sxs-lookup"><span data-stu-id="08f5a-123">version</span></span>|<span data-ttu-id="08f5a-124">2/4</span><span class="sxs-lookup"><span data-stu-id="08f5a-124">4</span></span>|<span data-ttu-id="08f5a-125">バージョン値の種類。</span><span class="sxs-lookup"><span data-stu-id="08f5a-125">Version value type.</span></span>|
|<span data-ttu-id="08f5a-126">sizeInMB</span><span class="sxs-lookup"><span data-stu-id="08f5a-126">sizeInMB</span></span>|<span data-ttu-id="08f5a-127">5</span><span class="sxs-lookup"><span data-stu-id="08f5a-127">5</span></span>|<span data-ttu-id="08f5a-128">サイズ検出の種類。</span><span class="sxs-lookup"><span data-stu-id="08f5a-128">Size detection type.</span></span>|
|<span data-ttu-id="08f5a-129">doesNotExist</span><span class="sxs-lookup"><span data-stu-id="08f5a-129">doesNotExist</span></span>|<span data-ttu-id="08f5a-130">シックス</span><span class="sxs-lookup"><span data-stu-id="08f5a-130">6</span></span>|<span data-ttu-id="08f5a-131">指定したファイルまたはフォルダーが存在しません。</span><span class="sxs-lookup"><span data-stu-id="08f5a-131">The specified file or folder does not exist.</span></span>|





