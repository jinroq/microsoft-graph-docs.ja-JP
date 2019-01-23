---
title: runState 列挙型
description: デバイスの管理スクリプトの実行ステータスの種類を示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4e83dbf367c1758c95ad02b0a0be8b5558e74f66
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425009"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="d8afe-103">runState 列挙型</span><span class="sxs-lookup"><span data-stu-id="d8afe-103">runState enum type</span></span>

> <span data-ttu-id="d8afe-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d8afe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8afe-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8afe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8afe-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8afe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8afe-107">デバイスの管理スクリプトの実行ステータスの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d8afe-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="d8afe-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d8afe-108">Members</span></span>
|<span data-ttu-id="d8afe-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d8afe-109">Member</span></span>|<span data-ttu-id="d8afe-110">値</span><span class="sxs-lookup"><span data-stu-id="d8afe-110">Value</span></span>|<span data-ttu-id="d8afe-111">説明</span><span class="sxs-lookup"><span data-stu-id="d8afe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8afe-112">不明</span><span class="sxs-lookup"><span data-stu-id="d8afe-112">unknown</span></span>|<span data-ttu-id="d8afe-113">0</span><span class="sxs-lookup"><span data-stu-id="d8afe-113">0</span></span>|<span data-ttu-id="d8afe-114">不明な結果です。</span><span class="sxs-lookup"><span data-stu-id="d8afe-114">Unknown result.</span></span>|
|<span data-ttu-id="d8afe-115">success</span><span class="sxs-lookup"><span data-stu-id="d8afe-115">success</span></span>|<span data-ttu-id="d8afe-116">1</span><span class="sxs-lookup"><span data-stu-id="d8afe-116">1</span></span>|<span data-ttu-id="d8afe-117">スクリプトが正常に実行します。</span><span class="sxs-lookup"><span data-stu-id="d8afe-117">Script is run successfully.</span></span>|
|<span data-ttu-id="d8afe-118">失敗します。</span><span class="sxs-lookup"><span data-stu-id="d8afe-118">fail</span></span>|<span data-ttu-id="d8afe-119">2</span><span class="sxs-lookup"><span data-stu-id="d8afe-119">2</span></span>|<span data-ttu-id="d8afe-120">スクリプトを実行できませんでした。</span><span class="sxs-lookup"><span data-stu-id="d8afe-120">Script failed to run.</span></span>|




