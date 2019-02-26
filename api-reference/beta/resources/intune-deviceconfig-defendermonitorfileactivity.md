---
title: defendermonitorfileactivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d04d7a34de9c08c12d17c994381683c160bef1c4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152592"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="56300-103">defendermonitorfileactivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="56300-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="56300-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56300-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56300-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="56300-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56300-106">ファイルアクティビティの監視に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="56300-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="56300-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="56300-107">Members</span></span>
|<span data-ttu-id="56300-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="56300-108">Member</span></span>|<span data-ttu-id="56300-109">値</span><span class="sxs-lookup"><span data-stu-id="56300-109">Value</span></span>|<span data-ttu-id="56300-110">説明</span><span class="sxs-lookup"><span data-stu-id="56300-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56300-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="56300-111">userDefined</span></span>|<span data-ttu-id="56300-112">.0</span><span class="sxs-lookup"><span data-stu-id="56300-112">0</span></span>|<span data-ttu-id="56300-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="56300-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="56300-114">無効にする</span><span class="sxs-lookup"><span data-stu-id="56300-114">disable</span></span>|<span data-ttu-id="56300-115">1-d</span><span class="sxs-lookup"><span data-stu-id="56300-115">1</span></span>|<span data-ttu-id="56300-116">ファイルの監視処理を無効にします。</span><span class="sxs-lookup"><span data-stu-id="56300-116">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="56300-117">monitorallfiles</span><span class="sxs-lookup"><span data-stu-id="56300-117">monitorAllFiles</span></span>|<span data-ttu-id="56300-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="56300-118">2</span></span>|<span data-ttu-id="56300-119">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="56300-119">Monitor all files.</span></span>|
|<span data-ttu-id="56300-120">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="56300-120">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="56300-121">1/3</span><span class="sxs-lookup"><span data-stu-id="56300-121">3</span></span>| <span data-ttu-id="56300-122">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="56300-122">Monitor incoming files only.</span></span>|
|<span data-ttu-id="56300-123">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="56300-123">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="56300-124">2/4</span><span class="sxs-lookup"><span data-stu-id="56300-124">4</span></span>|<span data-ttu-id="56300-125">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="56300-125">Monitor outgoing files only.</span></span>|




