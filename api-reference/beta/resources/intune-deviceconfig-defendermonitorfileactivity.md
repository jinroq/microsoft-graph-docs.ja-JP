---
title: defendermonitorfileactivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2888484f90bb3389fa7b7b12c79ce386d1bfd2db
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794331"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="1cd87-103">defendermonitorfileactivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="1cd87-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="1cd87-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cd87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cd87-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1cd87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cd87-106">ファイルアクティビティの監視に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="1cd87-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="1cd87-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1cd87-107">Members</span></span>
|<span data-ttu-id="1cd87-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1cd87-108">Member</span></span>|<span data-ttu-id="1cd87-109">値</span><span class="sxs-lookup"><span data-stu-id="1cd87-109">Value</span></span>|<span data-ttu-id="1cd87-110">説明</span><span class="sxs-lookup"><span data-stu-id="1cd87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd87-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="1cd87-111">userDefined</span></span>|<span data-ttu-id="1cd87-112">.0</span><span class="sxs-lookup"><span data-stu-id="1cd87-112">0</span></span>|<span data-ttu-id="1cd87-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="1cd87-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="1cd87-114">無効にする</span><span class="sxs-lookup"><span data-stu-id="1cd87-114">disable</span></span>|<span data-ttu-id="1cd87-115">1-d</span><span class="sxs-lookup"><span data-stu-id="1cd87-115">1</span></span>|<span data-ttu-id="1cd87-116">ファイルの監視処理を無効にします。</span><span class="sxs-lookup"><span data-stu-id="1cd87-116">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="1cd87-117">monitorallfiles</span><span class="sxs-lookup"><span data-stu-id="1cd87-117">monitorAllFiles</span></span>|<span data-ttu-id="1cd87-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="1cd87-118">2</span></span>|<span data-ttu-id="1cd87-119">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="1cd87-119">Monitor all files.</span></span>|
|<span data-ttu-id="1cd87-120">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="1cd87-120">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="1cd87-121">1/3</span><span class="sxs-lookup"><span data-stu-id="1cd87-121">3</span></span>| <span data-ttu-id="1cd87-122">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="1cd87-122">Monitor incoming files only.</span></span>|
|<span data-ttu-id="1cd87-123">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="1cd87-123">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="1cd87-124">2/4</span><span class="sxs-lookup"><span data-stu-id="1cd87-124">4</span></span>|<span data-ttu-id="1cd87-125">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="1cd87-125">Monitor outgoing files only.</span></span>|





