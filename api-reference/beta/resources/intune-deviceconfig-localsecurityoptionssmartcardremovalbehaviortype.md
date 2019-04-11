---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 785742f997df931cecb8144c127adf98ee74e58e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789487"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="103ec-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="103ec-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="103ec-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="103ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="103ec-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="103ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="103ec-106">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="103ec-106">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>

## <a name="members"></a><span data-ttu-id="103ec-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="103ec-107">Members</span></span>
|<span data-ttu-id="103ec-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="103ec-108">Member</span></span>|<span data-ttu-id="103ec-109">値</span><span class="sxs-lookup"><span data-stu-id="103ec-109">Value</span></span>|<span data-ttu-id="103ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="103ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="103ec-111">lockworkstation</span><span class="sxs-lookup"><span data-stu-id="103ec-111">lockWorkstation</span></span>|<span data-ttu-id="103ec-112">.0</span><span class="sxs-lookup"><span data-stu-id="103ec-112">0</span></span>|<span data-ttu-id="103ec-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="103ec-113">No Action</span></span>|
|<span data-ttu-id="103ec-114">noAction</span><span class="sxs-lookup"><span data-stu-id="103ec-114">noAction</span></span>|<span data-ttu-id="103ec-115">1-d</span><span class="sxs-lookup"><span data-stu-id="103ec-115">1</span></span>|<span data-ttu-id="103ec-116">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="103ec-116">Lock Workstation</span></span>|
|<span data-ttu-id="103ec-117">forcelogoff</span><span class="sxs-lookup"><span data-stu-id="103ec-117">forceLogoff</span></span>|<span data-ttu-id="103ec-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="103ec-118">2</span></span>|<span data-ttu-id="103ec-119">強制的にログオフ</span><span class="sxs-lookup"><span data-stu-id="103ec-119">Force Logoff</span></span>|
|<span data-ttu-id="103ec-120">切断 remotedesktopsession</span><span class="sxs-lookup"><span data-stu-id="103ec-120">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="103ec-121">1/3</span><span class="sxs-lookup"><span data-stu-id="103ec-121">3</span></span>|<span data-ttu-id="103ec-122">リモートリモートデスクトップサービスセッションの場合は切断する</span><span class="sxs-lookup"><span data-stu-id="103ec-122">Disconnect if a remote Remote Desktop Services session</span></span>|





