---
title: managedAppClipboardSharingLevel 列挙型
description: アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 349f0ee08b8e3bff4e627c58318e2c21fa00847c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946785"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="87e75-103">managedAppClipboardSharingLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="87e75-103">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="87e75-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="87e75-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87e75-105">アプリケーションとの間にデバイスのクリップボードを共有する可能性がありますレベルを表します</span><span class="sxs-lookup"><span data-stu-id="87e75-105">Represents the level to which the device's clipboard may be shared between apps</span></span>
## <a name="members"></a><span data-ttu-id="87e75-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="87e75-106">Members</span></span>
|<span data-ttu-id="87e75-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="87e75-107">Member</span></span>|<span data-ttu-id="87e75-108">値</span><span class="sxs-lookup"><span data-stu-id="87e75-108">Value</span></span>|<span data-ttu-id="87e75-109">説明</span><span class="sxs-lookup"><span data-stu-id="87e75-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87e75-110">allApps</span><span class="sxs-lookup"><span data-stu-id="87e75-110">allApps</span></span>|<span data-ttu-id="87e75-111">0</span><span class="sxs-lookup"><span data-stu-id="87e75-111">0</span></span>|<span data-ttu-id="87e75-112">かを管理するすべてのアプリケーション間での共有は</span><span class="sxs-lookup"><span data-stu-id="87e75-112">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="87e75-113">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="87e75-113">managedAppsWithPasteIn</span></span>|<span data-ttu-id="87e75-114">1</span><span class="sxs-lookup"><span data-stu-id="87e75-114">1</span></span>|<span data-ttu-id="87e75-115">共有間で許可されてすべてのマネージ アプリケーションでの貼り付けを有効になっています。</span><span class="sxs-lookup"><span data-stu-id="87e75-115">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="87e75-116">managedApps</span><span class="sxs-lookup"><span data-stu-id="87e75-116">managedApps</span></span>|<span data-ttu-id="87e75-117">2</span><span class="sxs-lookup"><span data-stu-id="87e75-117">2</span></span>|<span data-ttu-id="87e75-118">すべてのマネージ アプリケーションの間で許可を共有</span><span class="sxs-lookup"><span data-stu-id="87e75-118">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="87e75-119">ブロック</span><span class="sxs-lookup"><span data-stu-id="87e75-119">blocked</span></span>|<span data-ttu-id="87e75-120">3</span><span class="sxs-lookup"><span data-stu-id="87e75-120">3</span></span>|<span data-ttu-id="87e75-121">アプリケーション間での共有が無効になっています。</span><span class="sxs-lookup"><span data-stu-id="87e75-121">Sharing between apps is disabled</span></span>|



