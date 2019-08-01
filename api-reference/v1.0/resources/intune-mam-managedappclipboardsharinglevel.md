---
title: Managedappクリップボード Sharinglevel 列挙型
description: アプリケーション間でデバイスのクリップボードを共有するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58a1e50a77a468228b6218d620b589a6d25ca748
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038053"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="5926f-103">Managedappクリップボード Sharinglevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="5926f-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="5926f-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5926f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5926f-105">アプリケーション間でデバイスのクリップボードを共有するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="5926f-105">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="5926f-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="5926f-106">Members</span></span>
|<span data-ttu-id="5926f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5926f-107">Member</span></span>|<span data-ttu-id="5926f-108">値</span><span class="sxs-lookup"><span data-stu-id="5926f-108">Value</span></span>|<span data-ttu-id="5926f-109">説明</span><span class="sxs-lookup"><span data-stu-id="5926f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5926f-110">allApps</span><span class="sxs-lookup"><span data-stu-id="5926f-110">allApps</span></span>|<span data-ttu-id="5926f-111">.0</span><span class="sxs-lookup"><span data-stu-id="5926f-111">0</span></span>|<span data-ttu-id="5926f-112">すべてのアプリ間での共有が可能、管理されている</span><span class="sxs-lookup"><span data-stu-id="5926f-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="5926f-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="5926f-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="5926f-114">1-d</span><span class="sxs-lookup"><span data-stu-id="5926f-114">1</span></span>|<span data-ttu-id="5926f-115">[貼り付け] が有効になっているすべての管理対象アプリ間で共有が許可されます。</span><span class="sxs-lookup"><span data-stu-id="5926f-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="5926f-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="5926f-116">managedApps</span></span>|<span data-ttu-id="5926f-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5926f-117">2</span></span>|<span data-ttu-id="5926f-118">すべての管理対象アプリ間で共有が可能</span><span class="sxs-lookup"><span data-stu-id="5926f-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="5926f-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="5926f-119">blocked</span></span>|<span data-ttu-id="5926f-120">1/3</span><span class="sxs-lookup"><span data-stu-id="5926f-120">3</span></span>|<span data-ttu-id="5926f-121">アプリ間の共有が無効になっている</span><span class="sxs-lookup"><span data-stu-id="5926f-121">Sharing between apps is disabled</span></span>|



