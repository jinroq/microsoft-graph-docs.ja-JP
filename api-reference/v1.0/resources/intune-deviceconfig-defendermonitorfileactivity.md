---
title: defenderMonitorFileActivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c3a731f6e23c18c202c3baca3bd14e855152c558
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031851"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="c5abf-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="c5abf-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="c5abf-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5abf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5abf-105">ファイルアクティビティの監視に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="c5abf-105">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="c5abf-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="c5abf-106">Members</span></span>
|<span data-ttu-id="c5abf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c5abf-107">Member</span></span>|<span data-ttu-id="c5abf-108">値</span><span class="sxs-lookup"><span data-stu-id="c5abf-108">Value</span></span>|<span data-ttu-id="c5abf-109">説明</span><span class="sxs-lookup"><span data-stu-id="c5abf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5abf-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="c5abf-110">userDefined</span></span>|<span data-ttu-id="c5abf-111">.0</span><span class="sxs-lookup"><span data-stu-id="c5abf-111">0</span></span>|<span data-ttu-id="c5abf-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="c5abf-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c5abf-113">無効にする</span><span class="sxs-lookup"><span data-stu-id="c5abf-113">disable</span></span>|<span data-ttu-id="c5abf-114">1-d</span><span class="sxs-lookup"><span data-stu-id="c5abf-114">1</span></span>|<span data-ttu-id="c5abf-115">ファイルの監視処理を無効にします。</span><span class="sxs-lookup"><span data-stu-id="c5abf-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="c5abf-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="c5abf-116">monitorAllFiles</span></span>|<span data-ttu-id="c5abf-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="c5abf-117">2</span></span>|<span data-ttu-id="c5abf-118">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="c5abf-118">Monitor all files.</span></span>|
|<span data-ttu-id="c5abf-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="c5abf-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="c5abf-120">1/3</span><span class="sxs-lookup"><span data-stu-id="c5abf-120">3</span></span>| <span data-ttu-id="c5abf-121">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="c5abf-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="c5abf-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="c5abf-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="c5abf-123">2/4</span><span class="sxs-lookup"><span data-stu-id="c5abf-123">4</span></span>|<span data-ttu-id="c5abf-124">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="c5abf-124">Monitor outgoing files only.</span></span>|



