---
title: managedappクリップボード sharinglevel 列挙型
description: アプリケーション間でデバイスのクリップボードを共有するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 352a801c53acd487fdac0206eca828461d35bf68
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148350"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="c194c-103">managedappクリップボード sharinglevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="c194c-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="c194c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c194c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c194c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c194c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c194c-106">アプリケーション間でデバイスのクリップボードを共有するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="c194c-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="c194c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c194c-107">Members</span></span>
|<span data-ttu-id="c194c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c194c-108">Member</span></span>|<span data-ttu-id="c194c-109">値</span><span class="sxs-lookup"><span data-stu-id="c194c-109">Value</span></span>|<span data-ttu-id="c194c-110">説明</span><span class="sxs-lookup"><span data-stu-id="c194c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c194c-111">allapps</span><span class="sxs-lookup"><span data-stu-id="c194c-111">allApps</span></span>|<span data-ttu-id="c194c-112">.0</span><span class="sxs-lookup"><span data-stu-id="c194c-112">0</span></span>|<span data-ttu-id="c194c-113">すべてのアプリ間での共有が可能、管理されている</span><span class="sxs-lookup"><span data-stu-id="c194c-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="c194c-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="c194c-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="c194c-115">1-d</span><span class="sxs-lookup"><span data-stu-id="c194c-115">1</span></span>|<span data-ttu-id="c194c-116">[貼り付け] が有効になっているすべての管理対象アプリ間で共有が許可されます。</span><span class="sxs-lookup"><span data-stu-id="c194c-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="c194c-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="c194c-117">managedApps</span></span>|<span data-ttu-id="c194c-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c194c-118">2</span></span>|<span data-ttu-id="c194c-119">すべての管理対象アプリ間で共有が可能</span><span class="sxs-lookup"><span data-stu-id="c194c-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="c194c-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="c194c-120">blocked</span></span>|<span data-ttu-id="c194c-121">1/3</span><span class="sxs-lookup"><span data-stu-id="c194c-121">3</span></span>|<span data-ttu-id="c194c-122">アプリ間の共有が無効になっている</span><span class="sxs-lookup"><span data-stu-id="c194c-122">Sharing between apps is disabled</span></span>|




