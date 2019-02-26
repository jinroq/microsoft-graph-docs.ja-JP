---
title: defendermonitorfileactivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c53847d270639d11b5014291e62dde2668a4d5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256001"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="75ff6-103">defendermonitorfileactivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="75ff6-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="75ff6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75ff6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75ff6-105">ファイルアクティビティの監視に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="75ff6-105">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="75ff6-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="75ff6-106">Members</span></span>
|<span data-ttu-id="75ff6-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="75ff6-107">Member</span></span>|<span data-ttu-id="75ff6-108">値</span><span class="sxs-lookup"><span data-stu-id="75ff6-108">Value</span></span>|<span data-ttu-id="75ff6-109">説明</span><span class="sxs-lookup"><span data-stu-id="75ff6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75ff6-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="75ff6-110">userDefined</span></span>|<span data-ttu-id="75ff6-111">.0</span><span class="sxs-lookup"><span data-stu-id="75ff6-111">0</span></span>|<span data-ttu-id="75ff6-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="75ff6-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="75ff6-113">無効にする</span><span class="sxs-lookup"><span data-stu-id="75ff6-113">disable</span></span>|<span data-ttu-id="75ff6-114">1-d</span><span class="sxs-lookup"><span data-stu-id="75ff6-114">1</span></span>|<span data-ttu-id="75ff6-115">ファイルの監視処理を無効にします。</span><span class="sxs-lookup"><span data-stu-id="75ff6-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="75ff6-116">monitorallfiles</span><span class="sxs-lookup"><span data-stu-id="75ff6-116">monitorAllFiles</span></span>|<span data-ttu-id="75ff6-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="75ff6-117">2</span></span>|<span data-ttu-id="75ff6-118">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="75ff6-118">Monitor all files.</span></span>|
|<span data-ttu-id="75ff6-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="75ff6-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="75ff6-120">1/3</span><span class="sxs-lookup"><span data-stu-id="75ff6-120">3</span></span>| <span data-ttu-id="75ff6-121">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="75ff6-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="75ff6-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="75ff6-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="75ff6-123">2/4</span><span class="sxs-lookup"><span data-stu-id="75ff6-123">4</span></span>|<span data-ttu-id="75ff6-124">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="75ff6-124">Monitor outgoing files only.</span></span>|



