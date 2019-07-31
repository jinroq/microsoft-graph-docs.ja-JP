---
title: enrollmentState 列挙型
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4f394b02eac7e54c7e74a1c6954d6e3a7414e1b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999186"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="e1ac6-103">enrollmentState 列挙型</span><span class="sxs-lookup"><span data-stu-id="e1ac6-103">enrollmentState enum type</span></span>

> <span data-ttu-id="e1ac6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1ac6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1ac6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1ac6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1ac6-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e1ac6-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e1ac6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1ac6-107">Members</span></span>
|<span data-ttu-id="e1ac6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1ac6-108">Member</span></span>|<span data-ttu-id="e1ac6-109">値</span><span class="sxs-lookup"><span data-stu-id="e1ac6-109">Value</span></span>|<span data-ttu-id="e1ac6-110">説明</span><span class="sxs-lookup"><span data-stu-id="e1ac6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1ac6-111">不明</span><span class="sxs-lookup"><span data-stu-id="e1ac6-111">unknown</span></span>|<span data-ttu-id="e1ac6-112">.0</span><span class="sxs-lookup"><span data-stu-id="e1ac6-112">0</span></span>|<span data-ttu-id="e1ac6-113">デバイス登録の状態が不明です</span><span class="sxs-lookup"><span data-stu-id="e1ac6-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="e1ac6-114">遂げ</span><span class="sxs-lookup"><span data-stu-id="e1ac6-114">enrolled</span></span>|<span data-ttu-id="e1ac6-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e1ac6-115">1</span></span>|<span data-ttu-id="e1ac6-116">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="e1ac6-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="e1ac6-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="e1ac6-117">pendingReset</span></span>|<span data-ttu-id="e1ac6-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e1ac6-118">2</span></span>|<span data-ttu-id="e1ac6-119">登録済みですが、登録プロファイルによって登録され、登録されたプロファイルは割り当てられたプロファイルとは異なります。</span><span class="sxs-lookup"><span data-stu-id="e1ac6-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="e1ac6-120">フェール</span><span class="sxs-lookup"><span data-stu-id="e1ac6-120">failed</span></span>|<span data-ttu-id="e1ac6-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e1ac6-121">3</span></span>|<span data-ttu-id="e1ac6-122">登録されていません。登録エラーレコードがあります。</span><span class="sxs-lookup"><span data-stu-id="e1ac6-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="e1ac6-123">notContacted</span><span class="sxs-lookup"><span data-stu-id="e1ac6-123">notContacted</span></span>|<span data-ttu-id="e1ac6-124">2/4</span><span class="sxs-lookup"><span data-stu-id="e1ac6-124">4</span></span>|<span data-ttu-id="e1ac6-125">デバイスはインポートされていますが、登録されていません。</span><span class="sxs-lookup"><span data-stu-id="e1ac6-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="e1ac6-126">ブロック</span><span class="sxs-lookup"><span data-stu-id="e1ac6-126">blocked</span></span>|<span data-ttu-id="e1ac6-127">5</span><span class="sxs-lookup"><span data-stu-id="e1ac6-127">5</span></span>|<span data-ttu-id="e1ac6-128">デバイスは userless として登録されていますが、アプリのインストールが失敗したため、ユーザー登録への移動がブロックされています。</span><span class="sxs-lookup"><span data-stu-id="e1ac6-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





