---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2803e2d15b907fc2a05303be8a0b4e4db4ce66f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861454"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="89eee-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="89eee-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="89eee-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="89eee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89eee-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89eee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89eee-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89eee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89eee-107">Windows ユーザー アカウントに使用できる値は、設定を制御します。</span><span class="sxs-lookup"><span data-stu-id="89eee-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="89eee-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="89eee-108">Members</span></span>
|<span data-ttu-id="89eee-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="89eee-109">Member</span></span>|<span data-ttu-id="89eee-110">値</span><span class="sxs-lookup"><span data-stu-id="89eee-110">Value</span></span>|<span data-ttu-id="89eee-111">説明</span><span class="sxs-lookup"><span data-stu-id="89eee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89eee-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="89eee-112">userDefined</span></span>|<span data-ttu-id="89eee-113">0</span><span class="sxs-lookup"><span data-stu-id="89eee-113">0</span></span>|<span data-ttu-id="89eee-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="89eee-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="89eee-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="89eee-115">alwaysNotify</span></span>|<span data-ttu-id="89eee-116">1</span><span class="sxs-lookup"><span data-stu-id="89eee-116">1</span></span>|<span data-ttu-id="89eee-117">常に次のように通知します。</span><span class="sxs-lookup"><span data-stu-id="89eee-117">Always notify.</span></span>|
|<span data-ttu-id="89eee-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="89eee-118">notifyOnAppChanges</span></span>|<span data-ttu-id="89eee-119">2</span><span class="sxs-lookup"><span data-stu-id="89eee-119">2</span></span>|<span data-ttu-id="89eee-120">アプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="89eee-120">Notify on app changes.</span></span>|
|<span data-ttu-id="89eee-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="89eee-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="89eee-122">3</span><span class="sxs-lookup"><span data-stu-id="89eee-122">3</span></span>|<span data-ttu-id="89eee-123">デスクトップを暗転しないアプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="89eee-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="89eee-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="89eee-124">neverNotify</span></span>|<span data-ttu-id="89eee-125">4</span><span class="sxs-lookup"><span data-stu-id="89eee-125">4</span></span>|<span data-ttu-id="89eee-126">通知しません。</span><span class="sxs-lookup"><span data-stu-id="89eee-126">Never notify.</span></span>|





