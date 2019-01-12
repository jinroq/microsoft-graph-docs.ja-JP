---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd16db4236096687ddcc9f169dd657c938fd6815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911813"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="3fa8d-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="3fa8d-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="3fa8d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fa8d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fa8d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fa8d-107">Windows ユーザー アカウントに使用できる値は、設定を制御します。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-107">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="3fa8d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fa8d-108">Members</span></span>
|<span data-ttu-id="3fa8d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fa8d-109">Member</span></span>|<span data-ttu-id="3fa8d-110">値</span><span class="sxs-lookup"><span data-stu-id="3fa8d-110">Value</span></span>|<span data-ttu-id="3fa8d-111">説明</span><span class="sxs-lookup"><span data-stu-id="3fa8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fa8d-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="3fa8d-112">userDefined</span></span>|<span data-ttu-id="3fa8d-113">0</span><span class="sxs-lookup"><span data-stu-id="3fa8d-113">0</span></span>|<span data-ttu-id="3fa8d-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="3fa8d-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="3fa8d-115">alwaysNotify</span></span>|<span data-ttu-id="3fa8d-116">1</span><span class="sxs-lookup"><span data-stu-id="3fa8d-116">1</span></span>|<span data-ttu-id="3fa8d-117">常に次のように通知します。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-117">Always notify.</span></span>|
|<span data-ttu-id="3fa8d-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="3fa8d-118">notifyOnAppChanges</span></span>|<span data-ttu-id="3fa8d-119">2</span><span class="sxs-lookup"><span data-stu-id="3fa8d-119">2</span></span>|<span data-ttu-id="3fa8d-120">アプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-120">Notify on app changes.</span></span>|
|<span data-ttu-id="3fa8d-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="3fa8d-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="3fa8d-122">3</span><span class="sxs-lookup"><span data-stu-id="3fa8d-122">3</span></span>|<span data-ttu-id="3fa8d-123">デスクトップを暗転しないアプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="3fa8d-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="3fa8d-124">neverNotify</span></span>|<span data-ttu-id="3fa8d-125">4</span><span class="sxs-lookup"><span data-stu-id="3fa8d-125">4</span></span>|<span data-ttu-id="3fa8d-126">通知しません。</span><span class="sxs-lookup"><span data-stu-id="3fa8d-126">Never notify.</span></span>|





