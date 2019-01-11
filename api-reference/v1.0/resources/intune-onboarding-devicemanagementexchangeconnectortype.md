---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange コネクタの種類です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07449df53aa65036ae55e63c514c1687fbbab86a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888516"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="d3f87-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d3f87-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="d3f87-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3f87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3f87-105">Exchange コネクタの種類です。</span><span class="sxs-lookup"><span data-stu-id="d3f87-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="d3f87-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3f87-106">Members</span></span>
|<span data-ttu-id="d3f87-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d3f87-107">Member</span></span>|<span data-ttu-id="d3f87-108">値</span><span class="sxs-lookup"><span data-stu-id="d3f87-108">Value</span></span>|<span data-ttu-id="d3f87-109">説明</span><span class="sxs-lookup"><span data-stu-id="d3f87-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3f87-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="d3f87-110">onPremises</span></span>|<span data-ttu-id="d3f87-111">0</span><span class="sxs-lookup"><span data-stu-id="d3f87-111">0</span></span>|<span data-ttu-id="d3f87-112">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="d3f87-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="d3f87-113">ホスト</span><span class="sxs-lookup"><span data-stu-id="d3f87-113">hosted</span></span>|<span data-ttu-id="d3f87-114">1</span><span class="sxs-lookup"><span data-stu-id="d3f87-114">1</span></span>|<span data-ttu-id="d3f87-115">O365 マルチ テナント型の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="d3f87-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="d3f87-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="d3f87-116">serviceToService</span></span>|<span data-ttu-id="d3f87-117">2</span><span class="sxs-lookup"><span data-stu-id="d3f87-117">2</span></span>|<span data-ttu-id="d3f87-118">O365 マルチ テナント型の Exchange 環境に直接 Intune サービスに接続します。</span><span class="sxs-lookup"><span data-stu-id="d3f87-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="d3f87-119">専用</span><span class="sxs-lookup"><span data-stu-id="d3f87-119">dedicated</span></span>|<span data-ttu-id="d3f87-120">3</span><span class="sxs-lookup"><span data-stu-id="d3f87-120">3</span></span>|<span data-ttu-id="d3f87-121">O365 専用の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="d3f87-121">Connects to O365 Dedicated Exchange environment.</span></span>|



