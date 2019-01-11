---
title: managedAppClipboardSharingLevel 列挙型
description: アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します
localization_priority: Normal
ms.openlocfilehash: 16d6e9154b3d6e683d9ddce0efd70a40c01c8994
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814316"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="dd890-103">managedAppClipboardSharingLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="dd890-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="dd890-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd890-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd890-105">アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します</span><span class="sxs-lookup"><span data-stu-id="dd890-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="dd890-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="dd890-106">Members</span></span>
|<span data-ttu-id="dd890-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="dd890-107">Member</span></span>|<span data-ttu-id="dd890-108">値</span><span class="sxs-lookup"><span data-stu-id="dd890-108">Value</span></span>|<span data-ttu-id="dd890-109">説明</span><span class="sxs-lookup"><span data-stu-id="dd890-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd890-110">allApps</span><span class="sxs-lookup"><span data-stu-id="dd890-110">allApps</span></span>|<span data-ttu-id="dd890-111">0</span><span class="sxs-lookup"><span data-stu-id="dd890-111">0</span></span>|<span data-ttu-id="dd890-112">かを管理するすべてのアプリケーション間での共有は</span><span class="sxs-lookup"><span data-stu-id="dd890-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="dd890-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="dd890-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="dd890-114">1</span><span class="sxs-lookup"><span data-stu-id="dd890-114">1</span></span>|<span data-ttu-id="dd890-115">共有間で許可されてすべてのマネージ アプリケーションでの貼り付けを有効になっています。</span><span class="sxs-lookup"><span data-stu-id="dd890-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="dd890-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="dd890-116">managedApps</span></span>|<span data-ttu-id="dd890-117">2</span><span class="sxs-lookup"><span data-stu-id="dd890-117">2</span></span>|<span data-ttu-id="dd890-118">すべてのマネージ アプリケーションの間で許可を共有</span><span class="sxs-lookup"><span data-stu-id="dd890-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="dd890-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="dd890-119">blocked</span></span>|<span data-ttu-id="dd890-120">3</span><span class="sxs-lookup"><span data-stu-id="dd890-120">3</span></span>|<span data-ttu-id="dd890-121">アプリケーション間での共有が無効になっています。</span><span class="sxs-lookup"><span data-stu-id="dd890-121">Sharing between apps is disabled</span></span>|



