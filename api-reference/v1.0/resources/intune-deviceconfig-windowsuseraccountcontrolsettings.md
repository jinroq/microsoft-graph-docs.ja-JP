---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0475d8fb013cbb07f8d69a659f8ecde2eb580e43
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972475"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="d3938-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="d3938-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="d3938-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3938-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3938-105">Windows ユーザー アカウントに使用できる値は、設定を制御します。</span><span class="sxs-lookup"><span data-stu-id="d3938-105">Possible values for Windows user account control settings.</span></span>
## <a name="members"></a><span data-ttu-id="d3938-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3938-106">Members</span></span>
|<span data-ttu-id="d3938-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3938-107">Member</span></span>|<span data-ttu-id="d3938-108">値</span><span class="sxs-lookup"><span data-stu-id="d3938-108">Value</span></span>|<span data-ttu-id="d3938-109">説明</span><span class="sxs-lookup"><span data-stu-id="d3938-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3938-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="d3938-110">userDefined</span></span>|<span data-ttu-id="d3938-111">0</span><span class="sxs-lookup"><span data-stu-id="d3938-111">0</span></span>|<span data-ttu-id="d3938-112">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="d3938-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d3938-113">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="d3938-113">alwaysNotify</span></span>|<span data-ttu-id="d3938-114">1</span><span class="sxs-lookup"><span data-stu-id="d3938-114">1</span></span>|<span data-ttu-id="d3938-115">常に次のように通知します。</span><span class="sxs-lookup"><span data-stu-id="d3938-115">Always notify.</span></span>|
|<span data-ttu-id="d3938-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="d3938-116">notifyOnAppChanges</span></span>|<span data-ttu-id="d3938-117">2</span><span class="sxs-lookup"><span data-stu-id="d3938-117">2</span></span>|<span data-ttu-id="d3938-118">アプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="d3938-118">Notify on app changes.</span></span>|
|<span data-ttu-id="d3938-119">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="d3938-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="d3938-120">3</span><span class="sxs-lookup"><span data-stu-id="d3938-120">3</span></span>|<span data-ttu-id="d3938-121">デスクトップを暗転しないアプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="d3938-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="d3938-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="d3938-122">neverNotify</span></span>|<span data-ttu-id="d3938-123">4</span><span class="sxs-lookup"><span data-stu-id="d3938-123">4</span></span>|<span data-ttu-id="d3938-124">通知しません。</span><span class="sxs-lookup"><span data-stu-id="d3938-124">Never notify.</span></span>|



