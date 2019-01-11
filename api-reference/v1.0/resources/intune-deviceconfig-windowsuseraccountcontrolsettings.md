---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 02ea15b10b0eb6a789456d9f91e63ca3249a0933
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810662"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="06bf1-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="06bf1-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="06bf1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="06bf1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06bf1-105">Windows ユーザー アカウントに使用できる値は、設定を制御します。</span><span class="sxs-lookup"><span data-stu-id="06bf1-105">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="06bf1-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="06bf1-106">Members</span></span>
|<span data-ttu-id="06bf1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="06bf1-107">Member</span></span>|<span data-ttu-id="06bf1-108">値</span><span class="sxs-lookup"><span data-stu-id="06bf1-108">Value</span></span>|<span data-ttu-id="06bf1-109">説明</span><span class="sxs-lookup"><span data-stu-id="06bf1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06bf1-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="06bf1-110">userDefined</span></span>|<span data-ttu-id="06bf1-111">0</span><span class="sxs-lookup"><span data-stu-id="06bf1-111">0</span></span>|<span data-ttu-id="06bf1-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="06bf1-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="06bf1-113">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="06bf1-113">alwaysNotify</span></span>|<span data-ttu-id="06bf1-114">1</span><span class="sxs-lookup"><span data-stu-id="06bf1-114">1</span></span>|<span data-ttu-id="06bf1-115">常に次のように通知します。</span><span class="sxs-lookup"><span data-stu-id="06bf1-115">Always notify.</span></span>|
|<span data-ttu-id="06bf1-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="06bf1-116">notifyOnAppChanges</span></span>|<span data-ttu-id="06bf1-117">2</span><span class="sxs-lookup"><span data-stu-id="06bf1-117">2</span></span>|<span data-ttu-id="06bf1-118">アプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="06bf1-118">Notify on app changes.</span></span>|
|<span data-ttu-id="06bf1-119">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="06bf1-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="06bf1-120">3</span><span class="sxs-lookup"><span data-stu-id="06bf1-120">3</span></span>|<span data-ttu-id="06bf1-121">デスクトップを暗転しないアプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="06bf1-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="06bf1-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="06bf1-122">neverNotify</span></span>|<span data-ttu-id="06bf1-123">4</span><span class="sxs-lookup"><span data-stu-id="06bf1-123">4</span></span>|<span data-ttu-id="06bf1-124">通知しません。</span><span class="sxs-lookup"><span data-stu-id="06bf1-124">Never notify.</span></span>|



