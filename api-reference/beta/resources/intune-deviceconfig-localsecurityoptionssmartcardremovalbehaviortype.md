---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 65a3ad1828ec84dde1c9f5ab0fa8732862bc270c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946200"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="35a37-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="35a37-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="35a37-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35a37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35a37-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="35a37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35a37-106">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="35a37-106">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>

## <a name="members"></a><span data-ttu-id="35a37-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="35a37-107">Members</span></span>
|<span data-ttu-id="35a37-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="35a37-108">Member</span></span>|<span data-ttu-id="35a37-109">値</span><span class="sxs-lookup"><span data-stu-id="35a37-109">Value</span></span>|<span data-ttu-id="35a37-110">説明</span><span class="sxs-lookup"><span data-stu-id="35a37-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35a37-111">lockWorkstation</span><span class="sxs-lookup"><span data-stu-id="35a37-111">lockWorkstation</span></span>|<span data-ttu-id="35a37-112">.0</span><span class="sxs-lookup"><span data-stu-id="35a37-112">0</span></span>|<span data-ttu-id="35a37-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="35a37-113">No Action</span></span>|
|<span data-ttu-id="35a37-114">noAction</span><span class="sxs-lookup"><span data-stu-id="35a37-114">noAction</span></span>|<span data-ttu-id="35a37-115">1-d</span><span class="sxs-lookup"><span data-stu-id="35a37-115">1</span></span>|<span data-ttu-id="35a37-116">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="35a37-116">Lock Workstation</span></span>|
|<span data-ttu-id="35a37-117">forceLogoff</span><span class="sxs-lookup"><span data-stu-id="35a37-117">forceLogoff</span></span>|<span data-ttu-id="35a37-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="35a37-118">2</span></span>|<span data-ttu-id="35a37-119">強制的にログオフ</span><span class="sxs-lookup"><span data-stu-id="35a37-119">Force Logoff</span></span>|
|<span data-ttu-id="35a37-120">切断 Remotedesktopsession</span><span class="sxs-lookup"><span data-stu-id="35a37-120">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="35a37-121">1/3</span><span class="sxs-lookup"><span data-stu-id="35a37-121">3</span></span>|<span data-ttu-id="35a37-122">リモートリモートデスクトップサービスセッションの場合は切断する</span><span class="sxs-lookup"><span data-stu-id="35a37-122">Disconnect if a remote Remote Desktop Services session</span></span>|




