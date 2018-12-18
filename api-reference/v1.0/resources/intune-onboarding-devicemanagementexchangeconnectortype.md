---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange コネクタの種類です。
author: tfitzmac
ms.openlocfilehash: 333a5a7c6f73fead263edbdf3edafeefc3514ed1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306735"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="0102c-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0102c-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="0102c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0102c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0102c-105">Exchange コネクタの種類です。</span><span class="sxs-lookup"><span data-stu-id="0102c-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="0102c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0102c-106">Members</span></span>
|<span data-ttu-id="0102c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0102c-107">Member</span></span>|<span data-ttu-id="0102c-108">値</span><span class="sxs-lookup"><span data-stu-id="0102c-108">Value</span></span>|<span data-ttu-id="0102c-109">説明</span><span class="sxs-lookup"><span data-stu-id="0102c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0102c-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="0102c-110">onPremises</span></span>|<span data-ttu-id="0102c-111">0</span><span class="sxs-lookup"><span data-stu-id="0102c-111">0</span></span>|<span data-ttu-id="0102c-112">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="0102c-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="0102c-113">ホスト</span><span class="sxs-lookup"><span data-stu-id="0102c-113">hosted</span></span>|<span data-ttu-id="0102c-114">1</span><span class="sxs-lookup"><span data-stu-id="0102c-114">1</span></span>|<span data-ttu-id="0102c-115">O365 マルチ テナント型の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="0102c-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="0102c-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="0102c-116">serviceToService</span></span>|<span data-ttu-id="0102c-117">2</span><span class="sxs-lookup"><span data-stu-id="0102c-117">2</span></span>|<span data-ttu-id="0102c-118">O365 マルチ テナント型の Exchange 環境に直接 Intune サービスに接続します。</span><span class="sxs-lookup"><span data-stu-id="0102c-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="0102c-119">専用</span><span class="sxs-lookup"><span data-stu-id="0102c-119">dedicated</span></span>|<span data-ttu-id="0102c-120">3</span><span class="sxs-lookup"><span data-stu-id="0102c-120">3</span></span>|<span data-ttu-id="0102c-121">O365 専用の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="0102c-121">Connects to O365 Dedicated Exchange environment.</span></span>|



