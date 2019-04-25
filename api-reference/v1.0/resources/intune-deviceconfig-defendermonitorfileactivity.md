---
title: defendermonitorfileactivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c53847d270639d11b5014291e62dde2668a4d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534382"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="60543-103">defendermonitorfileactivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="60543-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="60543-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="60543-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60543-105">ファイルアクティビティの監視に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="60543-105">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="60543-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="60543-106">Members</span></span>
|<span data-ttu-id="60543-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="60543-107">Member</span></span>|<span data-ttu-id="60543-108">値</span><span class="sxs-lookup"><span data-stu-id="60543-108">Value</span></span>|<span data-ttu-id="60543-109">説明</span><span class="sxs-lookup"><span data-stu-id="60543-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60543-110">自分のもの</span><span class="sxs-lookup"><span data-stu-id="60543-110">userDefined</span></span>|<span data-ttu-id="60543-111">.0</span><span class="sxs-lookup"><span data-stu-id="60543-111">0</span></span>|<span data-ttu-id="60543-112">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="60543-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="60543-113">無効にする</span><span class="sxs-lookup"><span data-stu-id="60543-113">disable</span></span>|<span data-ttu-id="60543-114">1 </span><span class="sxs-lookup"><span data-stu-id="60543-114">1</span></span>|<span data-ttu-id="60543-115">ファイルの監視処理を無効にします。</span><span class="sxs-lookup"><span data-stu-id="60543-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="60543-116">monitorallfiles</span><span class="sxs-lookup"><span data-stu-id="60543-116">monitorAllFiles</span></span>|<span data-ttu-id="60543-117">2 </span><span class="sxs-lookup"><span data-stu-id="60543-117">2</span></span>|<span data-ttu-id="60543-118">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="60543-118">Monitor all files.</span></span>|
|<span data-ttu-id="60543-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="60543-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="60543-120">3 </span><span class="sxs-lookup"><span data-stu-id="60543-120">3</span></span>| <span data-ttu-id="60543-121">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="60543-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="60543-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="60543-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="60543-123">4 </span><span class="sxs-lookup"><span data-stu-id="60543-123">4</span></span>|<span data-ttu-id="60543-124">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="60543-124">Monitor outgoing files only.</span></span>|



