---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange Connector の現在の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 958cb848424d7d843a56b9414b6f8d9123398804
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037472"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="562bf-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="562bf-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="562bf-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="562bf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="562bf-105">Exchange Connector の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="562bf-105">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="562bf-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="562bf-106">Members</span></span>
|<span data-ttu-id="562bf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="562bf-107">Member</span></span>|<span data-ttu-id="562bf-108">値</span><span class="sxs-lookup"><span data-stu-id="562bf-108">Value</span></span>|<span data-ttu-id="562bf-109">説明</span><span class="sxs-lookup"><span data-stu-id="562bf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="562bf-110">none</span><span class="sxs-lookup"><span data-stu-id="562bf-110">none</span></span>|<span data-ttu-id="562bf-111">.0</span><span class="sxs-lookup"><span data-stu-id="562bf-111">0</span></span>|<span data-ttu-id="562bf-112">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="562bf-112">No Connector exists.</span></span>|
|<span data-ttu-id="562bf-113">connectionPending</span><span class="sxs-lookup"><span data-stu-id="562bf-113">connectionPending</span></span>|<span data-ttu-id="562bf-114">1-d</span><span class="sxs-lookup"><span data-stu-id="562bf-114">1</span></span>|<span data-ttu-id="562bf-115">Exchange 環境への保留中の接続。</span><span class="sxs-lookup"><span data-stu-id="562bf-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="562bf-116">まし</span><span class="sxs-lookup"><span data-stu-id="562bf-116">connected</span></span>|<span data-ttu-id="562bf-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="562bf-117">2</span></span>|<span data-ttu-id="562bf-118">Exchange 環境に接続されている</span><span class="sxs-lookup"><span data-stu-id="562bf-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="562bf-119">外す</span><span class="sxs-lookup"><span data-stu-id="562bf-119">disconnected</span></span>|<span data-ttu-id="562bf-120">1/3</span><span class="sxs-lookup"><span data-stu-id="562bf-120">3</span></span>|<span data-ttu-id="562bf-121">Exchange 環境から切断されている</span><span class="sxs-lookup"><span data-stu-id="562bf-121">Disconnected from the Exchange Environment</span></span>|



