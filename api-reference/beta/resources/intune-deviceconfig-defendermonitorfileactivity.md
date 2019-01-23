---
title: defenderMonitorFileActivity 列挙型
description: ファイル ・ アクティビティを監視するための可能な値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9b0f91d0a2d802fd573d7825da016dc8850e941
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414957"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="d0471-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="d0471-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="d0471-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0471-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d0471-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0471-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0471-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0471-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0471-107">ファイル ・ アクティビティを監視するための可能な値です。</span><span class="sxs-lookup"><span data-stu-id="d0471-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="d0471-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d0471-108">Members</span></span>
|<span data-ttu-id="d0471-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d0471-109">Member</span></span>|<span data-ttu-id="d0471-110">値</span><span class="sxs-lookup"><span data-stu-id="d0471-110">Value</span></span>|<span data-ttu-id="d0471-111">説明</span><span class="sxs-lookup"><span data-stu-id="d0471-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0471-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="d0471-112">userDefined</span></span>|<span data-ttu-id="d0471-113">0</span><span class="sxs-lookup"><span data-stu-id="d0471-113">0</span></span>|<span data-ttu-id="d0471-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="d0471-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d0471-115">無効にします。</span><span class="sxs-lookup"><span data-stu-id="d0471-115">disable</span></span>|<span data-ttu-id="d0471-116">1</span><span class="sxs-lookup"><span data-stu-id="d0471-116">1</span></span>|<span data-ttu-id="d0471-117">ファイル ・ アクティビティの監視を無効にします。</span><span class="sxs-lookup"><span data-stu-id="d0471-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="d0471-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="d0471-118">monitorAllFiles</span></span>|<span data-ttu-id="d0471-119">2</span><span class="sxs-lookup"><span data-stu-id="d0471-119">2</span></span>|<span data-ttu-id="d0471-120">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="d0471-120">Monitor all files.</span></span>|
|<span data-ttu-id="d0471-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="d0471-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="d0471-122">3</span><span class="sxs-lookup"><span data-stu-id="d0471-122">3</span></span>| <span data-ttu-id="d0471-123">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="d0471-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="d0471-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="d0471-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="d0471-125">4</span><span class="sxs-lookup"><span data-stu-id="d0471-125">4</span></span>|<span data-ttu-id="d0471-126">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="d0471-126">Monitor outgoing files only.</span></span>|




