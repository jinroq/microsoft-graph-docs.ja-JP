---
title: managedappクリップボード sharinglevel 列挙型
description: アプリケーション間でデバイスのクリップボードを共有するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcbee5e0b7aa6343e31d57d14557bc0f0586fb80
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465203"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="59c1f-103">managedappクリップボード sharinglevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="59c1f-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="59c1f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="59c1f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59c1f-105">アプリケーション間でデバイスのクリップボードを共有するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="59c1f-105">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="59c1f-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="59c1f-106">Members</span></span>
|<span data-ttu-id="59c1f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="59c1f-107">Member</span></span>|<span data-ttu-id="59c1f-108">値</span><span class="sxs-lookup"><span data-stu-id="59c1f-108">Value</span></span>|<span data-ttu-id="59c1f-109">説明</span><span class="sxs-lookup"><span data-stu-id="59c1f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59c1f-110">allapps</span><span class="sxs-lookup"><span data-stu-id="59c1f-110">allApps</span></span>|<span data-ttu-id="59c1f-111">.0</span><span class="sxs-lookup"><span data-stu-id="59c1f-111">0</span></span>|<span data-ttu-id="59c1f-112">すべてのアプリ間での共有が可能、管理されている</span><span class="sxs-lookup"><span data-stu-id="59c1f-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="59c1f-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="59c1f-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="59c1f-114">1-d</span><span class="sxs-lookup"><span data-stu-id="59c1f-114">1</span></span>|<span data-ttu-id="59c1f-115">[貼り付け] が有効になっているすべての管理対象アプリ間で共有が許可されます。</span><span class="sxs-lookup"><span data-stu-id="59c1f-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="59c1f-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="59c1f-116">managedApps</span></span>|<span data-ttu-id="59c1f-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="59c1f-117">2</span></span>|<span data-ttu-id="59c1f-118">すべての管理対象アプリ間で共有が可能</span><span class="sxs-lookup"><span data-stu-id="59c1f-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="59c1f-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="59c1f-119">blocked</span></span>|<span data-ttu-id="59c1f-120">1/3</span><span class="sxs-lookup"><span data-stu-id="59c1f-120">3</span></span>|<span data-ttu-id="59c1f-121">アプリ間の共有が無効になっている</span><span class="sxs-lookup"><span data-stu-id="59c1f-121">Sharing between apps is disabled</span></span>|



