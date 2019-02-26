---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18a7e37d0dcd38b44b1ba9edc22e026f6e4a7be7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163813"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="807cc-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="807cc-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="807cc-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="807cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="807cc-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="807cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="807cc-106">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="807cc-106">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>

## <a name="members"></a><span data-ttu-id="807cc-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="807cc-107">Members</span></span>
|<span data-ttu-id="807cc-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="807cc-108">Member</span></span>|<span data-ttu-id="807cc-109">値</span><span class="sxs-lookup"><span data-stu-id="807cc-109">Value</span></span>|<span data-ttu-id="807cc-110">説明</span><span class="sxs-lookup"><span data-stu-id="807cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="807cc-111">lockworkstation</span><span class="sxs-lookup"><span data-stu-id="807cc-111">lockWorkstation</span></span>|<span data-ttu-id="807cc-112">.0</span><span class="sxs-lookup"><span data-stu-id="807cc-112">0</span></span>|<span data-ttu-id="807cc-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="807cc-113">No Action</span></span>|
|<span data-ttu-id="807cc-114">noAction</span><span class="sxs-lookup"><span data-stu-id="807cc-114">noAction</span></span>|<span data-ttu-id="807cc-115">1-d</span><span class="sxs-lookup"><span data-stu-id="807cc-115">1</span></span>|<span data-ttu-id="807cc-116">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="807cc-116">Lock Workstation</span></span>|
|<span data-ttu-id="807cc-117">forcelogoff</span><span class="sxs-lookup"><span data-stu-id="807cc-117">forceLogoff</span></span>|<span data-ttu-id="807cc-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="807cc-118">2</span></span>|<span data-ttu-id="807cc-119">強制的にログオフ</span><span class="sxs-lookup"><span data-stu-id="807cc-119">Force Logoff</span></span>|
|<span data-ttu-id="807cc-120">切断 remotedesktopsession</span><span class="sxs-lookup"><span data-stu-id="807cc-120">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="807cc-121">1/3</span><span class="sxs-lookup"><span data-stu-id="807cc-121">3</span></span>|<span data-ttu-id="807cc-122">リモートリモートデスクトップサービスセッションの場合は切断する</span><span class="sxs-lookup"><span data-stu-id="807cc-122">Disconnect if a remote Remote Desktop Services session</span></span>|




