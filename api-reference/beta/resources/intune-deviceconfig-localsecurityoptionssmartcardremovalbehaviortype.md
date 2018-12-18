---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: tfitzmac
ms.openlocfilehash: 91b55d4ba3b1fc8b27a5ab85e6f5ff7df74e9a59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308737"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="e0856-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e0856-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="e0856-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e0856-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0856-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0856-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0856-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0856-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0856-107">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="e0856-107">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>
## <a name="members"></a><span data-ttu-id="e0856-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0856-108">Members</span></span>
|<span data-ttu-id="e0856-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="e0856-109">Member</span></span>|<span data-ttu-id="e0856-110">値</span><span class="sxs-lookup"><span data-stu-id="e0856-110">Value</span></span>|<span data-ttu-id="e0856-111">説明</span><span class="sxs-lookup"><span data-stu-id="e0856-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0856-112">lockWorkstation</span><span class="sxs-lookup"><span data-stu-id="e0856-112">lockWorkstation</span></span>|<span data-ttu-id="e0856-113">0</span><span class="sxs-lookup"><span data-stu-id="e0856-113">0</span></span>|<span data-ttu-id="e0856-114">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="e0856-114">No Action</span></span>|
|<span data-ttu-id="e0856-115">noAction</span><span class="sxs-lookup"><span data-stu-id="e0856-115">noAction</span></span>|<span data-ttu-id="e0856-116">1</span><span class="sxs-lookup"><span data-stu-id="e0856-116">1</span></span>|<span data-ttu-id="e0856-117">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="e0856-117">Lock Workstation</span></span>|
|<span data-ttu-id="e0856-118">forceLogoff</span><span class="sxs-lookup"><span data-stu-id="e0856-118">forceLogoff</span></span>|<span data-ttu-id="e0856-119">2</span><span class="sxs-lookup"><span data-stu-id="e0856-119">2</span></span>|<span data-ttu-id="e0856-120">ログオフを強制します。</span><span class="sxs-lookup"><span data-stu-id="e0856-120">Force Logoff</span></span>|
|<span data-ttu-id="e0856-121">disconnectRemoteDesktopSession</span><span class="sxs-lookup"><span data-stu-id="e0856-121">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="e0856-122">3</span><span class="sxs-lookup"><span data-stu-id="e0856-122">3</span></span>|<span data-ttu-id="e0856-123">場合、リモートのリモート デスクトップ サービス セッションを切断します。</span><span class="sxs-lookup"><span data-stu-id="e0856-123">Disconnect if a remote Remote Desktop Services session</span></span>|





