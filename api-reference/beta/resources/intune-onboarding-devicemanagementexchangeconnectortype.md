---
title: deviceManagementExchangeConnectorType 列挙型
description: Exchange コネクタの種類です。
author: tfitzmac
ms.openlocfilehash: 31459d4053e2ba1ef22a516995796baef2407dbf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301730"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="05ebc-103">deviceManagementExchangeConnectorType 列挙型</span><span class="sxs-lookup"><span data-stu-id="05ebc-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="05ebc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05ebc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05ebc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05ebc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05ebc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="05ebc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05ebc-107">Exchange コネクタの種類です。</span><span class="sxs-lookup"><span data-stu-id="05ebc-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="05ebc-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="05ebc-108">Members</span></span>
|<span data-ttu-id="05ebc-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="05ebc-109">Member</span></span>|<span data-ttu-id="05ebc-110">値</span><span class="sxs-lookup"><span data-stu-id="05ebc-110">Value</span></span>|<span data-ttu-id="05ebc-111">説明</span><span class="sxs-lookup"><span data-stu-id="05ebc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ebc-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="05ebc-112">onPremises</span></span>|<span data-ttu-id="05ebc-113">0</span><span class="sxs-lookup"><span data-stu-id="05ebc-113">0</span></span>|<span data-ttu-id="05ebc-114">オンプレミスの Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="05ebc-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="05ebc-115">ホスト</span><span class="sxs-lookup"><span data-stu-id="05ebc-115">hosted</span></span>|<span data-ttu-id="05ebc-116">1</span><span class="sxs-lookup"><span data-stu-id="05ebc-116">1</span></span>|<span data-ttu-id="05ebc-117">O365 マルチ テナント型の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="05ebc-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="05ebc-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="05ebc-118">serviceToService</span></span>|<span data-ttu-id="05ebc-119">2</span><span class="sxs-lookup"><span data-stu-id="05ebc-119">2</span></span>|<span data-ttu-id="05ebc-120">O365 マルチ テナント型の Exchange 環境に直接 Intune サービスに接続します。</span><span class="sxs-lookup"><span data-stu-id="05ebc-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="05ebc-121">専用</span><span class="sxs-lookup"><span data-stu-id="05ebc-121">dedicated</span></span>|<span data-ttu-id="05ebc-122">3</span><span class="sxs-lookup"><span data-stu-id="05ebc-122">3</span></span>|<span data-ttu-id="05ebc-123">O365 専用の Exchange 環境に接続します。</span><span class="sxs-lookup"><span data-stu-id="05ebc-123">Connects to O365 Dedicated Exchange environment.</span></span>|





