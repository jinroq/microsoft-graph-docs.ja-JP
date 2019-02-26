---
title: deviceManagementExchangeConnectorStatus 列挙型
description: Exchange Connector の現在の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472cc91b97547459694239c07bd211d1bd4ba1be
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260964"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="70e35-103">deviceManagementExchangeConnectorStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="70e35-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="70e35-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="70e35-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70e35-105">Exchange Connector の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="70e35-105">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="70e35-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="70e35-106">Members</span></span>
|<span data-ttu-id="70e35-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="70e35-107">Member</span></span>|<span data-ttu-id="70e35-108">値</span><span class="sxs-lookup"><span data-stu-id="70e35-108">Value</span></span>|<span data-ttu-id="70e35-109">説明</span><span class="sxs-lookup"><span data-stu-id="70e35-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70e35-110">none</span><span class="sxs-lookup"><span data-stu-id="70e35-110">none</span></span>|<span data-ttu-id="70e35-111">.0</span><span class="sxs-lookup"><span data-stu-id="70e35-111">0</span></span>|<span data-ttu-id="70e35-112">コネクタが存在しません。</span><span class="sxs-lookup"><span data-stu-id="70e35-112">No Connector exists.</span></span>|
|<span data-ttu-id="70e35-113">connectionpending</span><span class="sxs-lookup"><span data-stu-id="70e35-113">connectionPending</span></span>|<span data-ttu-id="70e35-114">1-d</span><span class="sxs-lookup"><span data-stu-id="70e35-114">1</span></span>|<span data-ttu-id="70e35-115">Exchange 環境への保留中の接続。</span><span class="sxs-lookup"><span data-stu-id="70e35-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="70e35-116">まし</span><span class="sxs-lookup"><span data-stu-id="70e35-116">connected</span></span>|<span data-ttu-id="70e35-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="70e35-117">2</span></span>|<span data-ttu-id="70e35-118">Exchange 環境に接続されている</span><span class="sxs-lookup"><span data-stu-id="70e35-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="70e35-119">外す</span><span class="sxs-lookup"><span data-stu-id="70e35-119">disconnected</span></span>|<span data-ttu-id="70e35-120">1/3</span><span class="sxs-lookup"><span data-stu-id="70e35-120">3</span></span>|<span data-ttu-id="70e35-121">Exchange 環境から切断されている</span><span class="sxs-lookup"><span data-stu-id="70e35-121">Disconnected from the Exchange Environment</span></span>|



