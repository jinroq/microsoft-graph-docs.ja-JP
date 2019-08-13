---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1315f7664b5966d276127bcdfabf9efc21b55355
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356670"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="ed4a9-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ed4a9-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="ed4a9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed4a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed4a9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ed4a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed4a9-106">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="ed4a9-106">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>

## <a name="members"></a><span data-ttu-id="ed4a9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ed4a9-107">Members</span></span>
|<span data-ttu-id="ed4a9-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ed4a9-108">Member</span></span>|<span data-ttu-id="ed4a9-109">値</span><span class="sxs-lookup"><span data-stu-id="ed4a9-109">Value</span></span>|<span data-ttu-id="ed4a9-110">説明</span><span class="sxs-lookup"><span data-stu-id="ed4a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed4a9-111">lockWorkstation</span><span class="sxs-lookup"><span data-stu-id="ed4a9-111">lockWorkstation</span></span>|<span data-ttu-id="ed4a9-112">.0</span><span class="sxs-lookup"><span data-stu-id="ed4a9-112">0</span></span>|<span data-ttu-id="ed4a9-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="ed4a9-113">No Action</span></span>|
|<span data-ttu-id="ed4a9-114">noAction</span><span class="sxs-lookup"><span data-stu-id="ed4a9-114">noAction</span></span>|<span data-ttu-id="ed4a9-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ed4a9-115">1</span></span>|<span data-ttu-id="ed4a9-116">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="ed4a9-116">Lock Workstation</span></span>|
|<span data-ttu-id="ed4a9-117">forceLogoff</span><span class="sxs-lookup"><span data-stu-id="ed4a9-117">forceLogoff</span></span>|<span data-ttu-id="ed4a9-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ed4a9-118">2</span></span>|<span data-ttu-id="ed4a9-119">強制的にログオフ</span><span class="sxs-lookup"><span data-stu-id="ed4a9-119">Force Logoff</span></span>|
|<span data-ttu-id="ed4a9-120">切断 Remotedesktopsession</span><span class="sxs-lookup"><span data-stu-id="ed4a9-120">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="ed4a9-121">1/3</span><span class="sxs-lookup"><span data-stu-id="ed4a9-121">3</span></span>|<span data-ttu-id="ed4a9-122">リモートリモートデスクトップサービスセッションの場合は切断する</span><span class="sxs-lookup"><span data-stu-id="ed4a9-122">Disconnect if a remote Remote Desktop Services session</span></span>|



