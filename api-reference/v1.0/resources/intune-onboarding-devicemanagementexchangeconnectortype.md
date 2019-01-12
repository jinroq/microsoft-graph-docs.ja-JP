---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange コネクタの種類です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e9e50a4475ca2d57b3f38567703046588d4fb3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986433"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="ede3a-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ede3a-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="ede3a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ede3a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ede3a-105">Exchange コネクタの種類です。</span><span class="sxs-lookup"><span data-stu-id="ede3a-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="ede3a-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ede3a-106">Members</span></span>
|<span data-ttu-id="ede3a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ede3a-107">Member</span></span>|<span data-ttu-id="ede3a-108">値</span><span class="sxs-lookup"><span data-stu-id="ede3a-108">Value</span></span>|<span data-ttu-id="ede3a-109">説明</span><span class="sxs-lookup"><span data-stu-id="ede3a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ede3a-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="ede3a-110">onPremises</span></span>|<span data-ttu-id="ede3a-111">0</span><span class="sxs-lookup"><span data-stu-id="ede3a-111">0</span></span>|<span data-ttu-id="ede3a-112">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="ede3a-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="ede3a-113">ホスト</span><span class="sxs-lookup"><span data-stu-id="ede3a-113">hosted</span></span>|<span data-ttu-id="ede3a-114">1</span><span class="sxs-lookup"><span data-stu-id="ede3a-114">1</span></span>|<span data-ttu-id="ede3a-115">O365 マルチ テナント型の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="ede3a-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="ede3a-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="ede3a-116">serviceToService</span></span>|<span data-ttu-id="ede3a-117">2</span><span class="sxs-lookup"><span data-stu-id="ede3a-117">2</span></span>|<span data-ttu-id="ede3a-118">O365 マルチ テナント型の Exchange 環境に直接 Intune サービスに接続します。</span><span class="sxs-lookup"><span data-stu-id="ede3a-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="ede3a-119">専用</span><span class="sxs-lookup"><span data-stu-id="ede3a-119">dedicated</span></span>|<span data-ttu-id="ede3a-120">3</span><span class="sxs-lookup"><span data-stu-id="ede3a-120">3</span></span>|<span data-ttu-id="ede3a-121">O365 専用の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="ede3a-121">Connects to O365 Dedicated Exchange environment.</span></span>|



