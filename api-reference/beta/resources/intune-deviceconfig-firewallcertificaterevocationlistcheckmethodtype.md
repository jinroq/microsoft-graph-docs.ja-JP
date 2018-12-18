---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
author: tfitzmac
ms.openlocfilehash: 302037187addfb8606c6c1e60a9369eb1f7c2ed5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320714"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="ea7de-103">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ea7de-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="ea7de-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ea7de-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea7de-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ea7de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea7de-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ea7de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea7de-107">FirewallCertificateRevocationListCheckMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="ea7de-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="ea7de-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ea7de-108">Members</span></span>
|<span data-ttu-id="ea7de-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ea7de-109">Member</span></span>|<span data-ttu-id="ea7de-110">値</span><span class="sxs-lookup"><span data-stu-id="ea7de-110">Value</span></span>|<span data-ttu-id="ea7de-111">説明</span><span class="sxs-lookup"><span data-stu-id="ea7de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea7de-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="ea7de-112">deviceDefault</span></span>|<span data-ttu-id="ea7de-113">0</span><span class="sxs-lookup"><span data-stu-id="ea7de-113">0</span></span>|<span data-ttu-id="ea7de-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="ea7de-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ea7de-115">none</span><span class="sxs-lookup"><span data-stu-id="ea7de-115">none</span></span>|<span data-ttu-id="ea7de-116">1</span><span class="sxs-lookup"><span data-stu-id="ea7de-116">1</span></span>|<span data-ttu-id="ea7de-117">証明書失効リストをチェックしません。</span><span class="sxs-lookup"><span data-stu-id="ea7de-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="ea7de-118">試行</span><span class="sxs-lookup"><span data-stu-id="ea7de-118">attempt</span></span>|<span data-ttu-id="ea7de-119">2</span><span class="sxs-lookup"><span data-stu-id="ea7de-119">2</span></span>|<span data-ttu-id="ea7de-120">CRL チェックを試みるし、チェックして、証明書が確認される場合にのみ証明書を許可します。</span><span class="sxs-lookup"><span data-stu-id="ea7de-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="ea7de-121">必要</span><span class="sxs-lookup"><span data-stu-id="ea7de-121">require</span></span>|<span data-ttu-id="ea7de-122">3</span><span class="sxs-lookup"><span data-stu-id="ea7de-122">3</span></span>|<span data-ttu-id="ea7de-123">証明書を許可する前に成功した CRL チェックが必要</span><span class="sxs-lookup"><span data-stu-id="ea7de-123">Require a successful CRL check before allowing a certificate</span></span>|





