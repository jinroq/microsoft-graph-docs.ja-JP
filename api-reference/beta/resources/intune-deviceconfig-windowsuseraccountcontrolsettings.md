---
title: windowsUserAccountControlSettings 列挙型
description: Windows ユーザー アカウントに使用できる値は、設定を制御します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ff348fd33e6bbc8370378783cf0a517a205ea101
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399816"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="569ee-103">windowsUserAccountControlSettings 列挙型</span><span class="sxs-lookup"><span data-stu-id="569ee-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="569ee-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="569ee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="569ee-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="569ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="569ee-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="569ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="569ee-107">Windows ユーザー アカウントに使用できる値は、設定を制御します。</span><span class="sxs-lookup"><span data-stu-id="569ee-107">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="569ee-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="569ee-108">Members</span></span>
|<span data-ttu-id="569ee-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="569ee-109">Member</span></span>|<span data-ttu-id="569ee-110">値</span><span class="sxs-lookup"><span data-stu-id="569ee-110">Value</span></span>|<span data-ttu-id="569ee-111">説明</span><span class="sxs-lookup"><span data-stu-id="569ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="569ee-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="569ee-112">userDefined</span></span>|<span data-ttu-id="569ee-113">0</span><span class="sxs-lookup"><span data-stu-id="569ee-113">0</span></span>|<span data-ttu-id="569ee-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="569ee-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="569ee-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="569ee-115">alwaysNotify</span></span>|<span data-ttu-id="569ee-116">1</span><span class="sxs-lookup"><span data-stu-id="569ee-116">1</span></span>|<span data-ttu-id="569ee-117">常に次のように通知します。</span><span class="sxs-lookup"><span data-stu-id="569ee-117">Always notify.</span></span>|
|<span data-ttu-id="569ee-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="569ee-118">notifyOnAppChanges</span></span>|<span data-ttu-id="569ee-119">2</span><span class="sxs-lookup"><span data-stu-id="569ee-119">2</span></span>|<span data-ttu-id="569ee-120">アプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="569ee-120">Notify on app changes.</span></span>|
|<span data-ttu-id="569ee-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="569ee-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="569ee-122">3</span><span class="sxs-lookup"><span data-stu-id="569ee-122">3</span></span>|<span data-ttu-id="569ee-123">デスクトップを暗転しないアプリケーションの変更を通知します。</span><span class="sxs-lookup"><span data-stu-id="569ee-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="569ee-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="569ee-124">neverNotify</span></span>|<span data-ttu-id="569ee-125">4</span><span class="sxs-lookup"><span data-stu-id="569ee-125">4</span></span>|<span data-ttu-id="569ee-126">通知しません。</span><span class="sxs-lookup"><span data-stu-id="569ee-126">Never notify.</span></span>|




