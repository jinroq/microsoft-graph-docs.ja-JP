---
title: deviceAppManagementTaskStatus 列挙型
description: デバイスアプリの管理タスクの状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3bcd6dcf957748a0e57776bd318cdb1ee734172
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002589"
---
# <a name="deviceappmanagementtaskstatus-enum-type"></a><span data-ttu-id="9d6de-103">deviceAppManagementTaskStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="9d6de-103">deviceAppManagementTaskStatus enum type</span></span>

> <span data-ttu-id="9d6de-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d6de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d6de-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d6de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d6de-106">デバイスアプリの管理タスクの状態。</span><span class="sxs-lookup"><span data-stu-id="9d6de-106">Device app management task status.</span></span>

## <a name="members"></a><span data-ttu-id="9d6de-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9d6de-107">Members</span></span>
|<span data-ttu-id="9d6de-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9d6de-108">Member</span></span>|<span data-ttu-id="9d6de-109">値</span><span class="sxs-lookup"><span data-stu-id="9d6de-109">Value</span></span>|<span data-ttu-id="9d6de-110">説明</span><span class="sxs-lookup"><span data-stu-id="9d6de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d6de-111">不明</span><span class="sxs-lookup"><span data-stu-id="9d6de-111">unknown</span></span>|<span data-ttu-id="9d6de-112">.0</span><span class="sxs-lookup"><span data-stu-id="9d6de-112">0</span></span>|<span data-ttu-id="9d6de-113">状態は未定義です。</span><span class="sxs-lookup"><span data-stu-id="9d6de-113">State is undefined.</span></span>|
|<span data-ttu-id="9d6de-114">対する</span><span class="sxs-lookup"><span data-stu-id="9d6de-114">pending</span></span>|<span data-ttu-id="9d6de-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9d6de-115">1</span></span>|<span data-ttu-id="9d6de-116">タスクをレビューできる状態にします。</span><span class="sxs-lookup"><span data-stu-id="9d6de-116">The task is ready for review.</span></span>|
|<span data-ttu-id="9d6de-117">active</span><span class="sxs-lookup"><span data-stu-id="9d6de-117">active</span></span>|<span data-ttu-id="9d6de-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9d6de-118">2</span></span>|<span data-ttu-id="9d6de-119">タスクは承諾され、作業中です。</span><span class="sxs-lookup"><span data-stu-id="9d6de-119">The task has been accepted and is being worked on.</span></span>|
|<span data-ttu-id="9d6de-120">せ</span><span class="sxs-lookup"><span data-stu-id="9d6de-120">completed</span></span>|<span data-ttu-id="9d6de-121">1/3</span><span class="sxs-lookup"><span data-stu-id="9d6de-121">3</span></span>|<span data-ttu-id="9d6de-122">作業は完了です。</span><span class="sxs-lookup"><span data-stu-id="9d6de-122">The work is complete.</span></span>|
|<span data-ttu-id="9d6de-123">拒否</span><span class="sxs-lookup"><span data-stu-id="9d6de-123">rejected</span></span>|<span data-ttu-id="9d6de-124">2/4</span><span class="sxs-lookup"><span data-stu-id="9d6de-124">4</span></span>|<span data-ttu-id="9d6de-125">タスクが拒否されました。</span><span class="sxs-lookup"><span data-stu-id="9d6de-125">The task was rejected.</span></span>|





