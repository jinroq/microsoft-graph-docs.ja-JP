---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6077bbecbb883dc1ca1eb55e92cd062444b25123
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973014"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="01ed2-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="01ed2-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="01ed2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="01ed2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01ed2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01ed2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01ed2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="01ed2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01ed2-107">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="01ed2-107">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>
## <a name="members"></a><span data-ttu-id="01ed2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="01ed2-108">Members</span></span>
|<span data-ttu-id="01ed2-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="01ed2-109">Member</span></span>|<span data-ttu-id="01ed2-110">値</span><span class="sxs-lookup"><span data-stu-id="01ed2-110">Value</span></span>|<span data-ttu-id="01ed2-111">説明</span><span class="sxs-lookup"><span data-stu-id="01ed2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01ed2-112">lockWorkstation</span><span class="sxs-lookup"><span data-stu-id="01ed2-112">lockWorkstation</span></span>|<span data-ttu-id="01ed2-113">0</span><span class="sxs-lookup"><span data-stu-id="01ed2-113">0</span></span>|<span data-ttu-id="01ed2-114">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="01ed2-114">No Action</span></span>|
|<span data-ttu-id="01ed2-115">noAction</span><span class="sxs-lookup"><span data-stu-id="01ed2-115">noAction</span></span>|<span data-ttu-id="01ed2-116">1</span><span class="sxs-lookup"><span data-stu-id="01ed2-116">1</span></span>|<span data-ttu-id="01ed2-117">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="01ed2-117">Lock Workstation</span></span>|
|<span data-ttu-id="01ed2-118">forceLogoff</span><span class="sxs-lookup"><span data-stu-id="01ed2-118">forceLogoff</span></span>|<span data-ttu-id="01ed2-119">2</span><span class="sxs-lookup"><span data-stu-id="01ed2-119">2</span></span>|<span data-ttu-id="01ed2-120">ログオフを強制します。</span><span class="sxs-lookup"><span data-stu-id="01ed2-120">Force Logoff</span></span>|
|<span data-ttu-id="01ed2-121">disconnectRemoteDesktopSession</span><span class="sxs-lookup"><span data-stu-id="01ed2-121">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="01ed2-122">3</span><span class="sxs-lookup"><span data-stu-id="01ed2-122">3</span></span>|<span data-ttu-id="01ed2-123">場合、リモートのリモート デスクトップ サービス セッションを切断します。</span><span class="sxs-lookup"><span data-stu-id="01ed2-123">Disconnect if a remote Remote Desktop Services session</span></span>|





