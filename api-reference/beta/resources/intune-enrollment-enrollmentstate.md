---
title: enrollmentState 列挙型
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: adb8c668bf3f6d30667417500a5989734167fb5c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992662"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="5a07f-103">enrollmentState 列挙型</span><span class="sxs-lookup"><span data-stu-id="5a07f-103">enrollmentState enum type</span></span>

> <span data-ttu-id="5a07f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a07f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a07f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a07f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a07f-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5a07f-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="5a07f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5a07f-107">Members</span></span>
|<span data-ttu-id="5a07f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5a07f-108">Member</span></span>|<span data-ttu-id="5a07f-109">値</span><span class="sxs-lookup"><span data-stu-id="5a07f-109">Value</span></span>|<span data-ttu-id="5a07f-110">説明</span><span class="sxs-lookup"><span data-stu-id="5a07f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a07f-111">不明</span><span class="sxs-lookup"><span data-stu-id="5a07f-111">unknown</span></span>|<span data-ttu-id="5a07f-112">.0</span><span class="sxs-lookup"><span data-stu-id="5a07f-112">0</span></span>|<span data-ttu-id="5a07f-113">デバイス登録の状態が不明です</span><span class="sxs-lookup"><span data-stu-id="5a07f-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="5a07f-114">遂げ</span><span class="sxs-lookup"><span data-stu-id="5a07f-114">enrolled</span></span>|<span data-ttu-id="5a07f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5a07f-115">1</span></span>|<span data-ttu-id="5a07f-116">デバイスは登録されています。</span><span class="sxs-lookup"><span data-stu-id="5a07f-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="5a07f-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="5a07f-117">pendingReset</span></span>|<span data-ttu-id="5a07f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5a07f-118">2</span></span>|<span data-ttu-id="5a07f-119">登録済みですが、登録プロファイルによって登録され、登録されたプロファイルは割り当てられたプロファイルとは異なります。</span><span class="sxs-lookup"><span data-stu-id="5a07f-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="5a07f-120">フェール</span><span class="sxs-lookup"><span data-stu-id="5a07f-120">failed</span></span>|<span data-ttu-id="5a07f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="5a07f-121">3</span></span>|<span data-ttu-id="5a07f-122">登録されていません。登録エラーレコードがあります。</span><span class="sxs-lookup"><span data-stu-id="5a07f-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="5a07f-123">notContacted</span><span class="sxs-lookup"><span data-stu-id="5a07f-123">notContacted</span></span>|<span data-ttu-id="5a07f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="5a07f-124">4</span></span>|<span data-ttu-id="5a07f-125">デバイスはインポートされていますが、登録されていません。</span><span class="sxs-lookup"><span data-stu-id="5a07f-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="5a07f-126">ブロック</span><span class="sxs-lookup"><span data-stu-id="5a07f-126">blocked</span></span>|<span data-ttu-id="5a07f-127">5</span><span class="sxs-lookup"><span data-stu-id="5a07f-127">5</span></span>|<span data-ttu-id="5a07f-128">デバイスは userless として登録されていますが、アプリのインストールが失敗したため、ユーザー登録への移動がブロックされています。</span><span class="sxs-lookup"><span data-stu-id="5a07f-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





