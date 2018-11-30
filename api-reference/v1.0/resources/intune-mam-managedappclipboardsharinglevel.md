---
title: managedAppClipboardSharingLevel 列挙型
description: アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します
ms.openlocfilehash: 7cf7b4a2f6ea6dc129a21167a2d75ba215ff29fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024233"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="6c71b-103">managedAppClipboardSharingLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="6c71b-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="6c71b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c71b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c71b-105">アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します</span><span class="sxs-lookup"><span data-stu-id="6c71b-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="6c71b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="6c71b-106">Members</span></span>
|<span data-ttu-id="6c71b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6c71b-107">Member</span></span>|<span data-ttu-id="6c71b-108">値</span><span class="sxs-lookup"><span data-stu-id="6c71b-108">Value</span></span>|<span data-ttu-id="6c71b-109">説明</span><span class="sxs-lookup"><span data-stu-id="6c71b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c71b-110">allApps</span><span class="sxs-lookup"><span data-stu-id="6c71b-110">allApps</span></span>|<span data-ttu-id="6c71b-111">0</span><span class="sxs-lookup"><span data-stu-id="6c71b-111">0</span></span>|<span data-ttu-id="6c71b-112">かを管理するすべてのアプリケーション間での共有は</span><span class="sxs-lookup"><span data-stu-id="6c71b-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="6c71b-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="6c71b-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="6c71b-114">1</span><span class="sxs-lookup"><span data-stu-id="6c71b-114">1</span></span>|<span data-ttu-id="6c71b-115">共有間で許可されてすべてのマネージ アプリケーションでの貼り付けを有効になっています。</span><span class="sxs-lookup"><span data-stu-id="6c71b-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="6c71b-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="6c71b-116">managedApps</span></span>|<span data-ttu-id="6c71b-117">2</span><span class="sxs-lookup"><span data-stu-id="6c71b-117">2</span></span>|<span data-ttu-id="6c71b-118">すべてのマネージ アプリケーションの間で許可を共有</span><span class="sxs-lookup"><span data-stu-id="6c71b-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="6c71b-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="6c71b-119">blocked</span></span>|<span data-ttu-id="6c71b-120">3</span><span class="sxs-lookup"><span data-stu-id="6c71b-120">3</span></span>|<span data-ttu-id="6c71b-121">アプリケーション間での共有が無効になっています。</span><span class="sxs-lookup"><span data-stu-id="6c71b-121">Sharing between apps is disabled</span></span>|



