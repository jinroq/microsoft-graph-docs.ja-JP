---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
ms.openlocfilehash: 4a4fdd6934805a688c95cd41f65149b4a727a60e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068250"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="5ba90-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5ba90-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="5ba90-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ba90-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ba90-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ba90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ba90-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ba90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ba90-107">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="5ba90-107">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>
## <a name="members"></a><span data-ttu-id="5ba90-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ba90-108">Members</span></span>
|<span data-ttu-id="5ba90-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ba90-109">Member</span></span>|<span data-ttu-id="5ba90-110">値</span><span class="sxs-lookup"><span data-stu-id="5ba90-110">Value</span></span>|<span data-ttu-id="5ba90-111">説明</span><span class="sxs-lookup"><span data-stu-id="5ba90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ba90-112">lockWorkstation</span><span class="sxs-lookup"><span data-stu-id="5ba90-112">lockWorkstation</span></span>|<span data-ttu-id="5ba90-113">0</span><span class="sxs-lookup"><span data-stu-id="5ba90-113">0</span></span>|<span data-ttu-id="5ba90-114">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="5ba90-114">No Action</span></span>|
|<span data-ttu-id="5ba90-115">noAction</span><span class="sxs-lookup"><span data-stu-id="5ba90-115">noAction</span></span>|<span data-ttu-id="5ba90-116">1</span><span class="sxs-lookup"><span data-stu-id="5ba90-116">1</span></span>|<span data-ttu-id="5ba90-117">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="5ba90-117">Lock Workstation</span></span>|
|<span data-ttu-id="5ba90-118">forceLogoff</span><span class="sxs-lookup"><span data-stu-id="5ba90-118">forceLogoff</span></span>|<span data-ttu-id="5ba90-119">2</span><span class="sxs-lookup"><span data-stu-id="5ba90-119">2</span></span>|<span data-ttu-id="5ba90-120">ログオフを強制します。</span><span class="sxs-lookup"><span data-stu-id="5ba90-120">Force Logoff</span></span>|
|<span data-ttu-id="5ba90-121">disconnectRemoteDesktopSession</span><span class="sxs-lookup"><span data-stu-id="5ba90-121">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="5ba90-122">3</span><span class="sxs-lookup"><span data-stu-id="5ba90-122">3</span></span>|<span data-ttu-id="5ba90-123">場合、リモートのリモート デスクトップ サービス セッションを切断します。</span><span class="sxs-lookup"><span data-stu-id="5ba90-123">Disconnect if a remote Remote Desktop Services session</span></span>|





