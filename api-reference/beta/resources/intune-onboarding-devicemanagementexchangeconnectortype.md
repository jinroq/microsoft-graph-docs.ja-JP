---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange コネクタの種類です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20eb1053d3dbf6cb657313f0c68f6c6c84804848
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398983"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="3651f-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3651f-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="3651f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3651f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3651f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3651f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3651f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3651f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3651f-107">Exchange コネクタの種類です。</span><span class="sxs-lookup"><span data-stu-id="3651f-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="3651f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3651f-108">Members</span></span>
|<span data-ttu-id="3651f-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="3651f-109">Member</span></span>|<span data-ttu-id="3651f-110">値</span><span class="sxs-lookup"><span data-stu-id="3651f-110">Value</span></span>|<span data-ttu-id="3651f-111">説明</span><span class="sxs-lookup"><span data-stu-id="3651f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3651f-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="3651f-112">onPremises</span></span>|<span data-ttu-id="3651f-113">0</span><span class="sxs-lookup"><span data-stu-id="3651f-113">0</span></span>|<span data-ttu-id="3651f-114">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="3651f-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="3651f-115">ホスト</span><span class="sxs-lookup"><span data-stu-id="3651f-115">hosted</span></span>|<span data-ttu-id="3651f-116">1</span><span class="sxs-lookup"><span data-stu-id="3651f-116">1</span></span>|<span data-ttu-id="3651f-117">O365 マルチ テナント型の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="3651f-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3651f-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="3651f-118">serviceToService</span></span>|<span data-ttu-id="3651f-119">2</span><span class="sxs-lookup"><span data-stu-id="3651f-119">2</span></span>|<span data-ttu-id="3651f-120">O365 マルチ テナント型の Exchange 環境に直接 Intune サービスに接続します。</span><span class="sxs-lookup"><span data-stu-id="3651f-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3651f-121">専用</span><span class="sxs-lookup"><span data-stu-id="3651f-121">dedicated</span></span>|<span data-ttu-id="3651f-122">3</span><span class="sxs-lookup"><span data-stu-id="3651f-122">3</span></span>|<span data-ttu-id="3651f-123">O365 専用の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="3651f-123">Connects to O365 Dedicated Exchange environment.</span></span>|




