---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 785742f997df931cecb8144c127adf98ee74e58e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460500"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="7a334-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7a334-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="7a334-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a334-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a334-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7a334-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a334-106">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="7a334-106">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>

## <a name="members"></a><span data-ttu-id="7a334-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7a334-107">Members</span></span>
|<span data-ttu-id="7a334-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7a334-108">Member</span></span>|<span data-ttu-id="7a334-109">値</span><span class="sxs-lookup"><span data-stu-id="7a334-109">Value</span></span>|<span data-ttu-id="7a334-110">説明</span><span class="sxs-lookup"><span data-stu-id="7a334-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a334-111">lockworkstation</span><span class="sxs-lookup"><span data-stu-id="7a334-111">lockWorkstation</span></span>|<span data-ttu-id="7a334-112">.0</span><span class="sxs-lookup"><span data-stu-id="7a334-112">0</span></span>|<span data-ttu-id="7a334-113">アクションなし</span><span class="sxs-lookup"><span data-stu-id="7a334-113">No Action</span></span>|
|<span data-ttu-id="7a334-114">noAction</span><span class="sxs-lookup"><span data-stu-id="7a334-114">noAction</span></span>|<span data-ttu-id="7a334-115">1-d</span><span class="sxs-lookup"><span data-stu-id="7a334-115">1</span></span>|<span data-ttu-id="7a334-116">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="7a334-116">Lock Workstation</span></span>|
|<span data-ttu-id="7a334-117">forcelogoff</span><span class="sxs-lookup"><span data-stu-id="7a334-117">forceLogoff</span></span>|<span data-ttu-id="7a334-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="7a334-118">2</span></span>|<span data-ttu-id="7a334-119">強制的にログオフ</span><span class="sxs-lookup"><span data-stu-id="7a334-119">Force Logoff</span></span>|
|<span data-ttu-id="7a334-120">切断 remotedesktopsession</span><span class="sxs-lookup"><span data-stu-id="7a334-120">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="7a334-121">1/3</span><span class="sxs-lookup"><span data-stu-id="7a334-121">3</span></span>|<span data-ttu-id="7a334-122">リモートリモートデスクトップサービスセッションの場合は切断する</span><span class="sxs-lookup"><span data-stu-id="7a334-122">Disconnect if a remote Remote Desktop Services session</span></span>|





