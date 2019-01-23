---
title: deviceManagementExchangeConnectorSyncType 列挙型
description: Exchange コネクタの同期要求の種類。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a78bf79990eb16ae6dbc62d4c324b905a79a7f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405626"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="d1c85-103">deviceManagementExchangeConnectorSyncType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d1c85-103">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="d1c85-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1c85-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d1c85-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1c85-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1c85-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1c85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1c85-107">Exchange コネクタの同期要求の種類。</span><span class="sxs-lookup"><span data-stu-id="d1c85-107">The type of Exchange Connector sync requested.</span></span>

## <a name="members"></a><span data-ttu-id="d1c85-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1c85-108">Members</span></span>
|<span data-ttu-id="d1c85-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d1c85-109">Member</span></span>|<span data-ttu-id="d1c85-110">値</span><span class="sxs-lookup"><span data-stu-id="d1c85-110">Value</span></span>|<span data-ttu-id="d1c85-111">説明</span><span class="sxs-lookup"><span data-stu-id="d1c85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1c85-112">fullSync</span><span class="sxs-lookup"><span data-stu-id="d1c85-112">fullSync</span></span>|<span data-ttu-id="d1c85-113">0</span><span class="sxs-lookup"><span data-stu-id="d1c85-113">0</span></span>|<span data-ttu-id="d1c85-114">Exchange のすべてのデバイスを検出します。</span><span class="sxs-lookup"><span data-stu-id="d1c85-114">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="d1c85-115">deltaSync</span><span class="sxs-lookup"><span data-stu-id="d1c85-115">deltaSync</span></span>|<span data-ttu-id="d1c85-116">1</span><span class="sxs-lookup"><span data-stu-id="d1c85-116">1</span></span>|<span data-ttu-id="d1c85-117">デルタ同期ウィンドウの中に更新する Exchange のデバイスのみを検出します。</span><span class="sxs-lookup"><span data-stu-id="d1c85-117">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|




