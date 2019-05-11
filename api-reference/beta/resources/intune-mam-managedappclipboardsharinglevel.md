---
title: Managedappクリップボード Sharinglevel 列挙型
description: アプリケーション間でデバイスのクリップボードを共有するレベルを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 298ed972967c01cd5c7ec66d59d78ee8d761c52b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940828"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="28c71-103">Managedappクリップボード Sharinglevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="28c71-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="28c71-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28c71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28c71-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="28c71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c71-106">アプリケーション間でデバイスのクリップボードを共有するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="28c71-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="28c71-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="28c71-107">Members</span></span>
|<span data-ttu-id="28c71-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="28c71-108">Member</span></span>|<span data-ttu-id="28c71-109">値</span><span class="sxs-lookup"><span data-stu-id="28c71-109">Value</span></span>|<span data-ttu-id="28c71-110">説明</span><span class="sxs-lookup"><span data-stu-id="28c71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c71-111">allApps</span><span class="sxs-lookup"><span data-stu-id="28c71-111">allApps</span></span>|<span data-ttu-id="28c71-112">.0</span><span class="sxs-lookup"><span data-stu-id="28c71-112">0</span></span>|<span data-ttu-id="28c71-113">すべてのアプリ間での共有が可能、管理されている</span><span class="sxs-lookup"><span data-stu-id="28c71-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="28c71-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="28c71-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="28c71-115">1-d</span><span class="sxs-lookup"><span data-stu-id="28c71-115">1</span></span>|<span data-ttu-id="28c71-116">[貼り付け] が有効になっているすべての管理対象アプリ間で共有が許可されます。</span><span class="sxs-lookup"><span data-stu-id="28c71-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="28c71-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="28c71-117">managedApps</span></span>|<span data-ttu-id="28c71-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="28c71-118">2</span></span>|<span data-ttu-id="28c71-119">すべての管理対象アプリ間で共有が可能</span><span class="sxs-lookup"><span data-stu-id="28c71-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="28c71-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="28c71-120">blocked</span></span>|<span data-ttu-id="28c71-121">1/3</span><span class="sxs-lookup"><span data-stu-id="28c71-121">3</span></span>|<span data-ttu-id="28c71-122">アプリ間の共有が無効になっている</span><span class="sxs-lookup"><span data-stu-id="28c71-122">Sharing between apps is disabled</span></span>|




