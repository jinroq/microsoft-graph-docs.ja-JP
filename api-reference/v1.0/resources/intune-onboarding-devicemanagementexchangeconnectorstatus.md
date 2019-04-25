---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange Connector の現在の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472cc91b97547459694239c07bd211d1bd4ba1be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565966"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="d3d8e-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="d3d8e-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="d3d8e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3d8e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3d8e-105">Exchange Connector の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="d3d8e-105">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="d3d8e-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3d8e-106">Members</span></span>
|<span data-ttu-id="d3d8e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3d8e-107">Member</span></span>|<span data-ttu-id="d3d8e-108">値</span><span class="sxs-lookup"><span data-stu-id="d3d8e-108">Value</span></span>|<span data-ttu-id="d3d8e-109">説明</span><span class="sxs-lookup"><span data-stu-id="d3d8e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d8e-110">なし</span><span class="sxs-lookup"><span data-stu-id="d3d8e-110">none</span></span>|<span data-ttu-id="d3d8e-111">.0</span><span class="sxs-lookup"><span data-stu-id="d3d8e-111">0</span></span>|<span data-ttu-id="d3d8e-112">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="d3d8e-112">No Connector exists.</span></span>|
|<span data-ttu-id="d3d8e-113">connectionpending</span><span class="sxs-lookup"><span data-stu-id="d3d8e-113">connectionPending</span></span>|<span data-ttu-id="d3d8e-114">1 </span><span class="sxs-lookup"><span data-stu-id="d3d8e-114">1</span></span>|<span data-ttu-id="d3d8e-115">Exchange 環境への保留中の接続。</span><span class="sxs-lookup"><span data-stu-id="d3d8e-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="d3d8e-116">まし</span><span class="sxs-lookup"><span data-stu-id="d3d8e-116">connected</span></span>|<span data-ttu-id="d3d8e-117">2 </span><span class="sxs-lookup"><span data-stu-id="d3d8e-117">2</span></span>|<span data-ttu-id="d3d8e-118">Exchange 環境に接続されている</span><span class="sxs-lookup"><span data-stu-id="d3d8e-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="d3d8e-119">外す</span><span class="sxs-lookup"><span data-stu-id="d3d8e-119">disconnected</span></span>|<span data-ttu-id="d3d8e-120">3 </span><span class="sxs-lookup"><span data-stu-id="d3d8e-120">3</span></span>|<span data-ttu-id="d3d8e-121">Exchange 環境から切断されている</span><span class="sxs-lookup"><span data-stu-id="d3d8e-121">Disconnected from the Exchange Environment</span></span>|



