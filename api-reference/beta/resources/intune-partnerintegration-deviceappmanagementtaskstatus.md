---
title: deviceAppManagementTaskStatus 列挙型
description: デバイスアプリの管理タスクの状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7e16d4904e8c81209190cca4ccd3d8304fcdfff2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308170"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a><span data-ttu-id="fedf6-103">deviceAppManagementTaskStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="fedf6-103">deviceAppManagementTaskStatus enum type</span></span>

> <span data-ttu-id="fedf6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fedf6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fedf6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fedf6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fedf6-106">デバイスアプリの管理タスクの状態。</span><span class="sxs-lookup"><span data-stu-id="fedf6-106">Device app management task status.</span></span>

## <a name="members"></a><span data-ttu-id="fedf6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="fedf6-107">Members</span></span>
|<span data-ttu-id="fedf6-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fedf6-108">Member</span></span>|<span data-ttu-id="fedf6-109">値</span><span class="sxs-lookup"><span data-stu-id="fedf6-109">Value</span></span>|<span data-ttu-id="fedf6-110">説明</span><span class="sxs-lookup"><span data-stu-id="fedf6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fedf6-111">不明</span><span class="sxs-lookup"><span data-stu-id="fedf6-111">unknown</span></span>|<span data-ttu-id="fedf6-112">.0</span><span class="sxs-lookup"><span data-stu-id="fedf6-112">0</span></span>|<span data-ttu-id="fedf6-113">状態は未定義です。</span><span class="sxs-lookup"><span data-stu-id="fedf6-113">State is undefined.</span></span>|
|<span data-ttu-id="fedf6-114">対する</span><span class="sxs-lookup"><span data-stu-id="fedf6-114">pending</span></span>|<span data-ttu-id="fedf6-115">1-d</span><span class="sxs-lookup"><span data-stu-id="fedf6-115">1</span></span>|<span data-ttu-id="fedf6-116">タスクをレビューできる状態にします。</span><span class="sxs-lookup"><span data-stu-id="fedf6-116">The task is ready for review.</span></span>|
|<span data-ttu-id="fedf6-117">active</span><span class="sxs-lookup"><span data-stu-id="fedf6-117">active</span></span>|<span data-ttu-id="fedf6-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="fedf6-118">2</span></span>|<span data-ttu-id="fedf6-119">タスクは承諾され、作業中です。</span><span class="sxs-lookup"><span data-stu-id="fedf6-119">The task has been accepted and is being worked on.</span></span>|
|<span data-ttu-id="fedf6-120">せ</span><span class="sxs-lookup"><span data-stu-id="fedf6-120">completed</span></span>|<span data-ttu-id="fedf6-121">1/3</span><span class="sxs-lookup"><span data-stu-id="fedf6-121">3</span></span>|<span data-ttu-id="fedf6-122">作業は完了です。</span><span class="sxs-lookup"><span data-stu-id="fedf6-122">The work is complete.</span></span>|
|<span data-ttu-id="fedf6-123">拒否</span><span class="sxs-lookup"><span data-stu-id="fedf6-123">rejected</span></span>|<span data-ttu-id="fedf6-124">2/4</span><span class="sxs-lookup"><span data-stu-id="fedf6-124">4</span></span>|<span data-ttu-id="fedf6-125">タスクが拒否されました。</span><span class="sxs-lookup"><span data-stu-id="fedf6-125">The task was rejected.</span></span>|



