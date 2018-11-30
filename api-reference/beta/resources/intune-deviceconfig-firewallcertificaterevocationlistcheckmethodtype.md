---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
ms.openlocfilehash: 425c4d6711bff2218f19303f746ff9e2b6a60033
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071666"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="71e2b-103">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="71e2b-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="71e2b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="71e2b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71e2b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71e2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71e2b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="71e2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71e2b-107">FirewallCertificateRevocationListCheckMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="71e2b-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="71e2b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="71e2b-108">Members</span></span>
|<span data-ttu-id="71e2b-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="71e2b-109">Member</span></span>|<span data-ttu-id="71e2b-110">値</span><span class="sxs-lookup"><span data-stu-id="71e2b-110">Value</span></span>|<span data-ttu-id="71e2b-111">説明</span><span class="sxs-lookup"><span data-stu-id="71e2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71e2b-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="71e2b-112">deviceDefault</span></span>|<span data-ttu-id="71e2b-113">0</span><span class="sxs-lookup"><span data-stu-id="71e2b-113">0</span></span>|<span data-ttu-id="71e2b-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="71e2b-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="71e2b-115">none</span><span class="sxs-lookup"><span data-stu-id="71e2b-115">none</span></span>|<span data-ttu-id="71e2b-116">1</span><span class="sxs-lookup"><span data-stu-id="71e2b-116">1</span></span>|<span data-ttu-id="71e2b-117">証明書失効リストをチェックしません。</span><span class="sxs-lookup"><span data-stu-id="71e2b-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="71e2b-118">試行</span><span class="sxs-lookup"><span data-stu-id="71e2b-118">attempt</span></span>|<span data-ttu-id="71e2b-119">2</span><span class="sxs-lookup"><span data-stu-id="71e2b-119">2</span></span>|<span data-ttu-id="71e2b-120">CRL チェックを試みるし、チェックして、証明書が確認される場合にのみ証明書を許可します。</span><span class="sxs-lookup"><span data-stu-id="71e2b-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="71e2b-121">必要</span><span class="sxs-lookup"><span data-stu-id="71e2b-121">require</span></span>|<span data-ttu-id="71e2b-122">3</span><span class="sxs-lookup"><span data-stu-id="71e2b-122">3</span></span>|<span data-ttu-id="71e2b-123">証明書を許可する前に成功した CRL チェックが必要</span><span class="sxs-lookup"><span data-stu-id="71e2b-123">Require a successful CRL check before allowing a certificate</span></span>|





