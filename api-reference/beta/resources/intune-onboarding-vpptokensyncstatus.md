---
title: vppTokenSyncStatus 列挙型
description: Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a53906018d45181bd16750e4ed3f0dac9dcb0d1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398815"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="d5d5c-103">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="d5d5c-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="d5d5c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5d5c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5d5c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5d5c-107">Apple ボリューム購入プログラム、トークンに関連付けられている可能性のある同期のステータス。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="d5d5c-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5d5c-108">Members</span></span>
|<span data-ttu-id="d5d5c-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5d5c-109">Member</span></span>|<span data-ttu-id="d5d5c-110">値</span><span class="sxs-lookup"><span data-stu-id="d5d5c-110">Value</span></span>|<span data-ttu-id="d5d5c-111">説明</span><span class="sxs-lookup"><span data-stu-id="d5d5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5d5c-112">none</span><span class="sxs-lookup"><span data-stu-id="d5d5c-112">none</span></span>|<span data-ttu-id="d5d5c-113">0</span><span class="sxs-lookup"><span data-stu-id="d5d5c-113">0</span></span>|<span data-ttu-id="d5d5c-114">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-114">Default status.</span></span>|
|<span data-ttu-id="d5d5c-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="d5d5c-115">inProgress</span></span>|<span data-ttu-id="d5d5c-116">1</span><span class="sxs-lookup"><span data-stu-id="d5d5c-116">1</span></span>|<span data-ttu-id="d5d5c-117">進行中の最後の同期します。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="d5d5c-118">完了</span><span class="sxs-lookup"><span data-stu-id="d5d5c-118">completed</span></span>|<span data-ttu-id="d5d5c-119">2</span><span class="sxs-lookup"><span data-stu-id="d5d5c-119">2</span></span>|<span data-ttu-id="d5d5c-120">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="d5d5c-121">失敗しました。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-121">failed</span></span>|<span data-ttu-id="d5d5c-122">3</span><span class="sxs-lookup"><span data-stu-id="d5d5c-122">3</span></span>|<span data-ttu-id="d5d5c-123">前回の同期が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="d5d5c-123">Last Sync failed.</span></span>|




