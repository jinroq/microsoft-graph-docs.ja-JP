---
title: defenderMonitorFileActivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09750eb4e9a6edda24006b7c7fd28d88f1ccd146
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947352"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="b4d58-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="b4d58-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="b4d58-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4d58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4d58-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b4d58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d58-106">ファイルアクティビティの監視に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="b4d58-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="b4d58-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b4d58-107">Members</span></span>
|<span data-ttu-id="b4d58-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b4d58-108">Member</span></span>|<span data-ttu-id="b4d58-109">値</span><span class="sxs-lookup"><span data-stu-id="b4d58-109">Value</span></span>|<span data-ttu-id="b4d58-110">説明</span><span class="sxs-lookup"><span data-stu-id="b4d58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d58-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="b4d58-111">userDefined</span></span>|<span data-ttu-id="b4d58-112">.0</span><span class="sxs-lookup"><span data-stu-id="b4d58-112">0</span></span>|<span data-ttu-id="b4d58-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="b4d58-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b4d58-114">無効にする</span><span class="sxs-lookup"><span data-stu-id="b4d58-114">disable</span></span>|<span data-ttu-id="b4d58-115">1-d</span><span class="sxs-lookup"><span data-stu-id="b4d58-115">1</span></span>|<span data-ttu-id="b4d58-116">ファイルの監視処理を無効にします。</span><span class="sxs-lookup"><span data-stu-id="b4d58-116">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="b4d58-117">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="b4d58-117">monitorAllFiles</span></span>|<span data-ttu-id="b4d58-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b4d58-118">2</span></span>|<span data-ttu-id="b4d58-119">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="b4d58-119">Monitor all files.</span></span>|
|<span data-ttu-id="b4d58-120">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="b4d58-120">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="b4d58-121">1/3</span><span class="sxs-lookup"><span data-stu-id="b4d58-121">3</span></span>| <span data-ttu-id="b4d58-122">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="b4d58-122">Monitor incoming files only.</span></span>|
|<span data-ttu-id="b4d58-123">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="b4d58-123">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="b4d58-124">2/4</span><span class="sxs-lookup"><span data-stu-id="b4d58-124">4</span></span>|<span data-ttu-id="b4d58-125">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="b4d58-125">Monitor outgoing files only.</span></span>|




