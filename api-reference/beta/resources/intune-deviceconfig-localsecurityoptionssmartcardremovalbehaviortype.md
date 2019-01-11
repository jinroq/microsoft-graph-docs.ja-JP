---
title: localSecurityOptionsSmartCardRemovalBehaviorType 列挙型
description: LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ab8ead80cc98a8036c4f874c61d541af09cbaaae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809969"
---
# <a name="localsecurityoptionssmartcardremovalbehaviortype-enum-type"></a><span data-ttu-id="84bd0-103">localSecurityOptionsSmartCardRemovalBehaviorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="84bd0-103">localSecurityOptionsSmartCardRemovalBehaviorType enum type</span></span>

> <span data-ttu-id="84bd0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84bd0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84bd0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84bd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84bd0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="84bd0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84bd0-107">LocalSecurityOptionsSmartCardRemovalBehaviorType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="84bd0-107">Possible values for LocalSecurityOptionsSmartCardRemovalBehaviorType</span></span>
## <a name="members"></a><span data-ttu-id="84bd0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="84bd0-108">Members</span></span>
|<span data-ttu-id="84bd0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="84bd0-109">Member</span></span>|<span data-ttu-id="84bd0-110">値</span><span class="sxs-lookup"><span data-stu-id="84bd0-110">Value</span></span>|<span data-ttu-id="84bd0-111">説明</span><span class="sxs-lookup"><span data-stu-id="84bd0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84bd0-112">lockWorkstation</span><span class="sxs-lookup"><span data-stu-id="84bd0-112">lockWorkstation</span></span>|<span data-ttu-id="84bd0-113">0</span><span class="sxs-lookup"><span data-stu-id="84bd0-113">0</span></span>|<span data-ttu-id="84bd0-114">操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="84bd0-114">No Action</span></span>|
|<span data-ttu-id="84bd0-115">noAction</span><span class="sxs-lookup"><span data-stu-id="84bd0-115">noAction</span></span>|<span data-ttu-id="84bd0-116">1</span><span class="sxs-lookup"><span data-stu-id="84bd0-116">1</span></span>|<span data-ttu-id="84bd0-117">ワークステーションのロック</span><span class="sxs-lookup"><span data-stu-id="84bd0-117">Lock Workstation</span></span>|
|<span data-ttu-id="84bd0-118">forceLogoff</span><span class="sxs-lookup"><span data-stu-id="84bd0-118">forceLogoff</span></span>|<span data-ttu-id="84bd0-119">2</span><span class="sxs-lookup"><span data-stu-id="84bd0-119">2</span></span>|<span data-ttu-id="84bd0-120">ログオフを強制します。</span><span class="sxs-lookup"><span data-stu-id="84bd0-120">Force Logoff</span></span>|
|<span data-ttu-id="84bd0-121">disconnectRemoteDesktopSession</span><span class="sxs-lookup"><span data-stu-id="84bd0-121">disconnectRemoteDesktopSession</span></span>|<span data-ttu-id="84bd0-122">3</span><span class="sxs-lookup"><span data-stu-id="84bd0-122">3</span></span>|<span data-ttu-id="84bd0-123">場合、リモートのリモート デスクトップ サービス セッションを切断します。</span><span class="sxs-lookup"><span data-stu-id="84bd0-123">Disconnect if a remote Remote Desktop Services session</span></span>|





