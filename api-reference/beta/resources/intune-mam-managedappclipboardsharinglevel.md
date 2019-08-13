---
title: Managedappクリップボード Sharinglevel 列挙型
description: アプリケーション間でデバイスのクリップボードを共有するレベルを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1e479f925e8b52ae746180851ce52ad116774367
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332212"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="257a0-103">Managedappクリップボード Sharinglevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="257a0-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="257a0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="257a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="257a0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="257a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="257a0-106">アプリケーション間でデバイスのクリップボードを共有するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="257a0-106">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="257a0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="257a0-107">Members</span></span>
|<span data-ttu-id="257a0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="257a0-108">Member</span></span>|<span data-ttu-id="257a0-109">値</span><span class="sxs-lookup"><span data-stu-id="257a0-109">Value</span></span>|<span data-ttu-id="257a0-110">説明</span><span class="sxs-lookup"><span data-stu-id="257a0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="257a0-111">allApps</span><span class="sxs-lookup"><span data-stu-id="257a0-111">allApps</span></span>|<span data-ttu-id="257a0-112">.0</span><span class="sxs-lookup"><span data-stu-id="257a0-112">0</span></span>|<span data-ttu-id="257a0-113">すべてのアプリ間での共有が可能、管理されている</span><span class="sxs-lookup"><span data-stu-id="257a0-113">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="257a0-114">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="257a0-114">managedAppsWithPasteIn</span></span>|<span data-ttu-id="257a0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="257a0-115">1</span></span>|<span data-ttu-id="257a0-116">[貼り付け] が有効になっているすべての管理対象アプリ間で共有が許可されます。</span><span class="sxs-lookup"><span data-stu-id="257a0-116">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="257a0-117">managedApps</span><span class="sxs-lookup"><span data-stu-id="257a0-117">managedApps</span></span>|<span data-ttu-id="257a0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="257a0-118">2</span></span>|<span data-ttu-id="257a0-119">すべての管理対象アプリ間で共有が可能</span><span class="sxs-lookup"><span data-stu-id="257a0-119">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="257a0-120">ブロック</span><span class="sxs-lookup"><span data-stu-id="257a0-120">blocked</span></span>|<span data-ttu-id="257a0-121">1/3</span><span class="sxs-lookup"><span data-stu-id="257a0-121">3</span></span>|<span data-ttu-id="257a0-122">アプリ間の共有が無効になっている</span><span class="sxs-lookup"><span data-stu-id="257a0-122">Sharing between apps is disabled</span></span>|



