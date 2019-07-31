---
title: defenderMonitorFileActivity 列挙型
description: ファイルアクティビティの監視に使用できる値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2039ca95b69f61b88e5b12b28b55977cb63c1b50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001783"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="97a87-103">defenderMonitorFileActivity 列挙型</span><span class="sxs-lookup"><span data-stu-id="97a87-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="97a87-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97a87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97a87-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97a87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97a87-106">ファイルアクティビティの監視に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="97a87-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="97a87-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="97a87-107">Members</span></span>
|<span data-ttu-id="97a87-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="97a87-108">Member</span></span>|<span data-ttu-id="97a87-109">値</span><span class="sxs-lookup"><span data-stu-id="97a87-109">Value</span></span>|<span data-ttu-id="97a87-110">説明</span><span class="sxs-lookup"><span data-stu-id="97a87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97a87-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="97a87-111">userDefined</span></span>|<span data-ttu-id="97a87-112">.0</span><span class="sxs-lookup"><span data-stu-id="97a87-112">0</span></span>|<span data-ttu-id="97a87-113">ユーザー定義、既定値、意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="97a87-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="97a87-114">無効にする</span><span class="sxs-lookup"><span data-stu-id="97a87-114">disable</span></span>|<span data-ttu-id="97a87-115">1-d</span><span class="sxs-lookup"><span data-stu-id="97a87-115">1</span></span>|<span data-ttu-id="97a87-116">ファイルの監視処理を無効にします。</span><span class="sxs-lookup"><span data-stu-id="97a87-116">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="97a87-117">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="97a87-117">monitorAllFiles</span></span>|<span data-ttu-id="97a87-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="97a87-118">2</span></span>|<span data-ttu-id="97a87-119">すべてのファイルを監視します。</span><span class="sxs-lookup"><span data-stu-id="97a87-119">Monitor all files.</span></span>|
|<span data-ttu-id="97a87-120">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="97a87-120">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="97a87-121">1/3</span><span class="sxs-lookup"><span data-stu-id="97a87-121">3</span></span>| <span data-ttu-id="97a87-122">受信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="97a87-122">Monitor incoming files only.</span></span>|
|<span data-ttu-id="97a87-123">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="97a87-123">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="97a87-124">2/4</span><span class="sxs-lookup"><span data-stu-id="97a87-124">4</span></span>|<span data-ttu-id="97a87-125">送信ファイルのみを監視します。</span><span class="sxs-lookup"><span data-stu-id="97a87-125">Monitor outgoing files only.</span></span>|





