---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3891f358efe3049af7cb53dbcd4f6c658190d235
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970228"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="341a7-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="341a7-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="341a7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="341a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="341a7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="341a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="341a7-106">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="341a7-106">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>

## <a name="members"></a><span data-ttu-id="341a7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="341a7-107">Members</span></span>
|<span data-ttu-id="341a7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="341a7-108">Member</span></span>|<span data-ttu-id="341a7-109">値</span><span class="sxs-lookup"><span data-stu-id="341a7-109">Value</span></span>|<span data-ttu-id="341a7-110">説明</span><span class="sxs-lookup"><span data-stu-id="341a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="341a7-111">lockWorkstation</span><span class="sxs-lookup"><span data-stu-id="341a7-111">lockWorkstation</span></span>|<span data-ttu-id="341a7-112">.0</span><span class="sxs-lookup"><span data-stu-id="341a7-112">0</span></span>|<span data-ttu-id="341a7-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="341a7-113">No Action</span></span>|
|<span data-ttu-id="341a7-114">noAction</span><span class="sxs-lookup"><span data-stu-id="341a7-114">noAction</span></span>|<span data-ttu-id="341a7-115">1-d</span><span class="sxs-lookup"><span data-stu-id="341a7-115">1</span></span>|<span data-ttu-id="341a7-116">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="341a7-116">Lock Workstation</span></span>|
|<span data-ttu-id="341a7-117">forceLogoff</span><span class="sxs-lookup"><span data-stu-id="341a7-117">forceLogoff</span></span>|<span data-ttu-id="341a7-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="341a7-118">2</span></span>|<span data-ttu-id="341a7-119">強制的にログオフ</span><span class="sxs-lookup"><span data-stu-id="341a7-119">Force Logoff</span></span>|
|<span data-ttu-id="341a7-120">切断 Remotedesktopsession</span><span class="sxs-lookup"><span data-stu-id="341a7-120">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="341a7-121">1/3</span><span class="sxs-lookup"><span data-stu-id="341a7-121">3</span></span>|<span data-ttu-id="341a7-122">リモートリモートデスクトップサービスセッションの場合は切断する</span><span class="sxs-lookup"><span data-stu-id="341a7-122">Disconnect if a remote Remote Desktop Services session</span></span>|





