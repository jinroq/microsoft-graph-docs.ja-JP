---
title: managedAppClipboardSharingLevel 列挙型
description: アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ccd90e4d704a075eaf43650fa765fabf3ab0b99
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410988"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="e75c8-103">managedAppClipboardSharingLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="e75c8-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="e75c8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e75c8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e75c8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e75c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e75c8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e75c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e75c8-107">アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します</span><span class="sxs-lookup"><span data-stu-id="e75c8-107">Represents the level to which the device's clipboard may be shared between apps</span></span>

## <a name="members"></a><span data-ttu-id="e75c8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e75c8-108">Members</span></span>
|<span data-ttu-id="e75c8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e75c8-109">Member</span></span>|<span data-ttu-id="e75c8-110">値</span><span class="sxs-lookup"><span data-stu-id="e75c8-110">Value</span></span>|<span data-ttu-id="e75c8-111">説明</span><span class="sxs-lookup"><span data-stu-id="e75c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e75c8-112">allApps</span><span class="sxs-lookup"><span data-stu-id="e75c8-112">allApps</span></span>|<span data-ttu-id="e75c8-113">0</span><span class="sxs-lookup"><span data-stu-id="e75c8-113">0</span></span>|<span data-ttu-id="e75c8-114">かを管理するすべてのアプリケーション間での共有は</span><span class="sxs-lookup"><span data-stu-id="e75c8-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="e75c8-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="e75c8-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="e75c8-116">1</span><span class="sxs-lookup"><span data-stu-id="e75c8-116">1</span></span>|<span data-ttu-id="e75c8-117">共有間で許可されてすべてのマネージ アプリケーションでの貼り付けを有効になっています。</span><span class="sxs-lookup"><span data-stu-id="e75c8-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="e75c8-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="e75c8-118">managedApps</span></span>|<span data-ttu-id="e75c8-119">2</span><span class="sxs-lookup"><span data-stu-id="e75c8-119">2</span></span>|<span data-ttu-id="e75c8-120">すべてのマネージ アプリケーションの間で許可を共有</span><span class="sxs-lookup"><span data-stu-id="e75c8-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="e75c8-121">ブロック</span><span class="sxs-lookup"><span data-stu-id="e75c8-121">blocked</span></span>|<span data-ttu-id="e75c8-122">3</span><span class="sxs-lookup"><span data-stu-id="e75c8-122">3</span></span>|<span data-ttu-id="e75c8-123">アプリケーション間での共有が無効になっています。</span><span class="sxs-lookup"><span data-stu-id="e75c8-123">Sharing between apps is disabled</span></span>|




