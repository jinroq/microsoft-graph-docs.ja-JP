---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
author: tfitzmac
ms.openlocfilehash: 33e9c914e9c816257cebbebe3754865c5ef17db7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358073"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="28317-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="28317-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="28317-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="28317-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28317-105">Windows ユーザー アカウントに使用できる値は、設定を制御します。</span><span class="sxs-lookup"><span data-stu-id="28317-105">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="28317-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="28317-106">Members</span></span>
|<span data-ttu-id="28317-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="28317-107">Member</span></span>|<span data-ttu-id="28317-108">値</span><span class="sxs-lookup"><span data-stu-id="28317-108">Value</span></span>|<span data-ttu-id="28317-109">説明</span><span class="sxs-lookup"><span data-stu-id="28317-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28317-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="28317-110">userDefined</span></span>|<span data-ttu-id="28317-111">0</span><span class="sxs-lookup"><span data-stu-id="28317-111">0</span></span>|<span data-ttu-id="28317-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="28317-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="28317-113">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="28317-113">alwaysNotify</span></span>|<span data-ttu-id="28317-114">1</span><span class="sxs-lookup"><span data-stu-id="28317-114">1</span></span>|<span data-ttu-id="28317-115">常に次のように通知します。</span><span class="sxs-lookup"><span data-stu-id="28317-115">Always notify.</span></span>|
|<span data-ttu-id="28317-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="28317-116">notifyOnAppChanges</span></span>|<span data-ttu-id="28317-117">2</span><span class="sxs-lookup"><span data-stu-id="28317-117">2</span></span>|<span data-ttu-id="28317-118">アプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="28317-118">Notify on app changes.</span></span>|
|<span data-ttu-id="28317-119">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="28317-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="28317-120">3</span><span class="sxs-lookup"><span data-stu-id="28317-120">3</span></span>|<span data-ttu-id="28317-121">デスクトップを暗転しないアプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="28317-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="28317-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="28317-122">neverNotify</span></span>|<span data-ttu-id="28317-123">4</span><span class="sxs-lookup"><span data-stu-id="28317-123">4</span></span>|<span data-ttu-id="28317-124">通知しません。</span><span class="sxs-lookup"><span data-stu-id="28317-124">Never notify.</span></span>|



