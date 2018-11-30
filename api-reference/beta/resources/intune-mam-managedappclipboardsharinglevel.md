---
title: managedAppClipboardSharingLevel 列挙型
description: アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します
ms.openlocfilehash: 71c4ab2d629fdfee3ded68612d7060a0fa069809
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073944"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="617e1-103">managedAppClipboardSharingLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="617e1-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="617e1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="617e1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="617e1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="617e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="617e1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="617e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="617e1-107">アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します</span><span class="sxs-lookup"><span data-stu-id="617e1-107">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="617e1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="617e1-108">Members</span></span>
|<span data-ttu-id="617e1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="617e1-109">Member</span></span>|<span data-ttu-id="617e1-110">値</span><span class="sxs-lookup"><span data-stu-id="617e1-110">Value</span></span>|<span data-ttu-id="617e1-111">説明</span><span class="sxs-lookup"><span data-stu-id="617e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="617e1-112">allApps</span><span class="sxs-lookup"><span data-stu-id="617e1-112">allApps</span></span>|<span data-ttu-id="617e1-113">0</span><span class="sxs-lookup"><span data-stu-id="617e1-113">0</span></span>|<span data-ttu-id="617e1-114">かを管理するすべてのアプリケーション間での共有は</span><span class="sxs-lookup"><span data-stu-id="617e1-114">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="617e1-115">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="617e1-115">managedAppsWithPasteIn</span></span>|<span data-ttu-id="617e1-116">1</span><span class="sxs-lookup"><span data-stu-id="617e1-116">1</span></span>|<span data-ttu-id="617e1-117">共有間で許可されてすべてのマネージ アプリケーションでの貼り付けを有効になっています。</span><span class="sxs-lookup"><span data-stu-id="617e1-117">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="617e1-118">managedApps</span><span class="sxs-lookup"><span data-stu-id="617e1-118">managedApps</span></span>|<span data-ttu-id="617e1-119">2</span><span class="sxs-lookup"><span data-stu-id="617e1-119">2</span></span>|<span data-ttu-id="617e1-120">すべてのマネージ アプリケーションの間で許可を共有</span><span class="sxs-lookup"><span data-stu-id="617e1-120">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="617e1-121">ブロック</span><span class="sxs-lookup"><span data-stu-id="617e1-121">blocked</span></span>|<span data-ttu-id="617e1-122">3</span><span class="sxs-lookup"><span data-stu-id="617e1-122">3</span></span>|<span data-ttu-id="617e1-123">アプリケーション間での共有が無効になっています。</span><span class="sxs-lookup"><span data-stu-id="617e1-123">Sharing between apps is disabled</span></span>|





