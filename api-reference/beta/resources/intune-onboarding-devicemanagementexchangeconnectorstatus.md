---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange コネクタの現在の状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 16181c49b05c74ef680f456b4bffd11b435299fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397772"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="2f261-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="2f261-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="2f261-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2f261-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f261-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f261-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f261-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f261-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f261-107">Exchange コネクタの現在の状態です。</span><span class="sxs-lookup"><span data-stu-id="2f261-107">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="2f261-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="2f261-108">Members</span></span>
|<span data-ttu-id="2f261-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="2f261-109">Member</span></span>|<span data-ttu-id="2f261-110">値</span><span class="sxs-lookup"><span data-stu-id="2f261-110">Value</span></span>|<span data-ttu-id="2f261-111">説明</span><span class="sxs-lookup"><span data-stu-id="2f261-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f261-112">none</span><span class="sxs-lookup"><span data-stu-id="2f261-112">none</span></span>|<span data-ttu-id="2f261-113">0</span><span class="sxs-lookup"><span data-stu-id="2f261-113">0</span></span>|<span data-ttu-id="2f261-114">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="2f261-114">No Connector exists.</span></span>|
|<span data-ttu-id="2f261-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="2f261-115">connectionPending</span></span>|<span data-ttu-id="2f261-116">1</span><span class="sxs-lookup"><span data-stu-id="2f261-116">1</span></span>|<span data-ttu-id="2f261-117">Exchange 環境に対して保留中の接続です。</span><span class="sxs-lookup"><span data-stu-id="2f261-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="2f261-118">接続されています。</span><span class="sxs-lookup"><span data-stu-id="2f261-118">connected</span></span>|<span data-ttu-id="2f261-119">2</span><span class="sxs-lookup"><span data-stu-id="2f261-119">2</span></span>|<span data-ttu-id="2f261-120">Exchange 環境に接続されています。</span><span class="sxs-lookup"><span data-stu-id="2f261-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="2f261-121">切断</span><span class="sxs-lookup"><span data-stu-id="2f261-121">disconnected</span></span>|<span data-ttu-id="2f261-122">3</span><span class="sxs-lookup"><span data-stu-id="2f261-122">3</span></span>|<span data-ttu-id="2f261-123">Exchange 環境から切断されています。</span><span class="sxs-lookup"><span data-stu-id="2f261-123">Disconnected from the Exchange Environment</span></span>|




