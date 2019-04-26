---
title: defendermonitorfileactivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2888484f90bb3389fa7b7b12c79ce386d1bfd2db
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563505"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="20ebd-103">defendermonitorfileactivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="20ebd-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="20ebd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20ebd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20ebd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="20ebd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20ebd-106">ファイルアクティビティの監視に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="20ebd-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="20ebd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="20ebd-107">Members</span></span>
|<span data-ttu-id="20ebd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="20ebd-108">Member</span></span>|<span data-ttu-id="20ebd-109">値</span><span class="sxs-lookup"><span data-stu-id="20ebd-109">Value</span></span>|<span data-ttu-id="20ebd-110">説明</span><span class="sxs-lookup"><span data-stu-id="20ebd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20ebd-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="20ebd-111">userDefined</span></span>|<span data-ttu-id="20ebd-112">.0</span><span class="sxs-lookup"><span data-stu-id="20ebd-112">0</span></span>|<span data-ttu-id="20ebd-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="20ebd-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="20ebd-114">無効にする</span><span class="sxs-lookup"><span data-stu-id="20ebd-114">disable</span></span>|<span data-ttu-id="20ebd-115">1 </span><span class="sxs-lookup"><span data-stu-id="20ebd-115">1</span></span>|<span data-ttu-id="20ebd-116">ファイルの監視処理を無効にします。</span><span class="sxs-lookup"><span data-stu-id="20ebd-116">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="20ebd-117">monitorallfiles</span><span class="sxs-lookup"><span data-stu-id="20ebd-117">monitorAllFiles</span></span>|<span data-ttu-id="20ebd-118">2 </span><span class="sxs-lookup"><span data-stu-id="20ebd-118">2</span></span>|<span data-ttu-id="20ebd-119">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="20ebd-119">Monitor all files.</span></span>|
|<span data-ttu-id="20ebd-120">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="20ebd-120">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="20ebd-121">3 </span><span class="sxs-lookup"><span data-stu-id="20ebd-121">3</span></span>| <span data-ttu-id="20ebd-122">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="20ebd-122">Monitor incoming files only.</span></span>|
|<span data-ttu-id="20ebd-123">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="20ebd-123">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="20ebd-124">4 </span><span class="sxs-lookup"><span data-stu-id="20ebd-124">4</span></span>|<span data-ttu-id="20ebd-125">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="20ebd-125">Monitor outgoing files only.</span></span>|





