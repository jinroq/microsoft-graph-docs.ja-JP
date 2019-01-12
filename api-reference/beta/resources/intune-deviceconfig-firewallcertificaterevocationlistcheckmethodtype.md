---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 915fab77e7a2c28ab9d6902f3e1cb7d2d05cb2b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958412"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="a227e-103">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a227e-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="a227e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a227e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a227e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a227e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a227e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a227e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a227e-107">FirewallCertificateRevocationListCheckMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="a227e-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="a227e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a227e-108">Members</span></span>
|<span data-ttu-id="a227e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a227e-109">Member</span></span>|<span data-ttu-id="a227e-110">値</span><span class="sxs-lookup"><span data-stu-id="a227e-110">Value</span></span>|<span data-ttu-id="a227e-111">説明</span><span class="sxs-lookup"><span data-stu-id="a227e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a227e-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a227e-112">deviceDefault</span></span>|<span data-ttu-id="a227e-113">0</span><span class="sxs-lookup"><span data-stu-id="a227e-113">0</span></span>|<span data-ttu-id="a227e-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="a227e-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="a227e-115">none</span><span class="sxs-lookup"><span data-stu-id="a227e-115">none</span></span>|<span data-ttu-id="a227e-116">1</span><span class="sxs-lookup"><span data-stu-id="a227e-116">1</span></span>|<span data-ttu-id="a227e-117">証明書失効リストをチェックしません。</span><span class="sxs-lookup"><span data-stu-id="a227e-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="a227e-118">試行</span><span class="sxs-lookup"><span data-stu-id="a227e-118">attempt</span></span>|<span data-ttu-id="a227e-119">2</span><span class="sxs-lookup"><span data-stu-id="a227e-119">2</span></span>|<span data-ttu-id="a227e-120">CRL チェックを試みるし、チェックして、証明書が確認される場合にのみ証明書を許可します。</span><span class="sxs-lookup"><span data-stu-id="a227e-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="a227e-121">必要</span><span class="sxs-lookup"><span data-stu-id="a227e-121">require</span></span>|<span data-ttu-id="a227e-122">3</span><span class="sxs-lookup"><span data-stu-id="a227e-122">3</span></span>|<span data-ttu-id="a227e-123">証明書を許可する前に成功した CRL チェックが必要</span><span class="sxs-lookup"><span data-stu-id="a227e-123">Require a successful CRL check before allowing a certificate</span></span>|





