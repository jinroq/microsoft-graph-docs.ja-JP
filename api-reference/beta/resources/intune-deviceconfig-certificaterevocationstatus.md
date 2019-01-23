---
title: certificateRevocationStatus 列挙型
description: 証明書失効の状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 373cb6247a695a5912d02d4fb1a353c40aeac581
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421971"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="8fc43-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="8fc43-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="8fc43-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8fc43-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8fc43-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fc43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fc43-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8fc43-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fc43-107">証明書失効の状態です。</span><span class="sxs-lookup"><span data-stu-id="8fc43-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="8fc43-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="8fc43-108">Members</span></span>
|<span data-ttu-id="8fc43-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="8fc43-109">Member</span></span>|<span data-ttu-id="8fc43-110">値</span><span class="sxs-lookup"><span data-stu-id="8fc43-110">Value</span></span>|<span data-ttu-id="8fc43-111">説明</span><span class="sxs-lookup"><span data-stu-id="8fc43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fc43-112">none</span><span class="sxs-lookup"><span data-stu-id="8fc43-112">none</span></span>|<span data-ttu-id="8fc43-113">0</span><span class="sxs-lookup"><span data-stu-id="8fc43-113">0</span></span>|<span data-ttu-id="8fc43-114">失効していません。</span><span class="sxs-lookup"><span data-stu-id="8fc43-114">Not revoked.</span></span>|
|<span data-ttu-id="8fc43-115">保留中</span><span class="sxs-lookup"><span data-stu-id="8fc43-115">pending</span></span>|<span data-ttu-id="8fc43-116">1</span><span class="sxs-lookup"><span data-stu-id="8fc43-116">1</span></span>|<span data-ttu-id="8fc43-117">保留中の失効します。</span><span class="sxs-lookup"><span data-stu-id="8fc43-117">Revocation pending.</span></span>|
|<span data-ttu-id="8fc43-118">発行</span><span class="sxs-lookup"><span data-stu-id="8fc43-118">issued</span></span>|<span data-ttu-id="8fc43-119">2</span><span class="sxs-lookup"><span data-stu-id="8fc43-119">2</span></span>|<span data-ttu-id="8fc43-120">取り消しコマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="8fc43-120">Revocation command issued.</span></span>|
|<span data-ttu-id="8fc43-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="8fc43-121">failed</span></span>|<span data-ttu-id="8fc43-122">3</span><span class="sxs-lookup"><span data-stu-id="8fc43-122">3</span></span>|<span data-ttu-id="8fc43-123">失効が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="8fc43-123">Revocation failed.</span></span>|
|<span data-ttu-id="8fc43-124">失効</span><span class="sxs-lookup"><span data-stu-id="8fc43-124">revoked</span></span>|<span data-ttu-id="8fc43-125">4</span><span class="sxs-lookup"><span data-stu-id="8fc43-125">4</span></span>|<span data-ttu-id="8fc43-126">無効にします。</span><span class="sxs-lookup"><span data-stu-id="8fc43-126">Revoked.</span></span>|




