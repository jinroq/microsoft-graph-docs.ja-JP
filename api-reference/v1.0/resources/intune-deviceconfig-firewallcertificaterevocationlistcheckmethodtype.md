---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e479b10339ab515a17f67d85de0c8d43c1507825
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940058"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="28a23-103">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="28a23-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="28a23-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="28a23-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28a23-105">FirewallCertificateRevocationListCheckMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="28a23-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="28a23-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="28a23-106">Members</span></span>
|<span data-ttu-id="28a23-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="28a23-107">Member</span></span>|<span data-ttu-id="28a23-108">値</span><span class="sxs-lookup"><span data-stu-id="28a23-108">Value</span></span>|<span data-ttu-id="28a23-109">説明</span><span class="sxs-lookup"><span data-stu-id="28a23-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28a23-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="28a23-110">deviceDefault</span></span>|<span data-ttu-id="28a23-111">0</span><span class="sxs-lookup"><span data-stu-id="28a23-111">0</span></span>|<span data-ttu-id="28a23-112">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="28a23-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="28a23-113">none</span><span class="sxs-lookup"><span data-stu-id="28a23-113">none</span></span>|<span data-ttu-id="28a23-114">1</span><span class="sxs-lookup"><span data-stu-id="28a23-114">1</span></span>|<span data-ttu-id="28a23-115">証明書失効リストをチェックしません。</span><span class="sxs-lookup"><span data-stu-id="28a23-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="28a23-116">試行</span><span class="sxs-lookup"><span data-stu-id="28a23-116">attempt</span></span>|<span data-ttu-id="28a23-117">2</span><span class="sxs-lookup"><span data-stu-id="28a23-117">2</span></span>|<span data-ttu-id="28a23-118">CRL チェックを試みるし、チェックして、証明書が確認される場合にのみ証明書を許可します。</span><span class="sxs-lookup"><span data-stu-id="28a23-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="28a23-119">必要</span><span class="sxs-lookup"><span data-stu-id="28a23-119">require</span></span>|<span data-ttu-id="28a23-120">3</span><span class="sxs-lookup"><span data-stu-id="28a23-120">3</span></span>|<span data-ttu-id="28a23-121">証明書を許可する前に成功した CRL チェックが必要</span><span class="sxs-lookup"><span data-stu-id="28a23-121">Require a successful CRL check before allowing a certificate</span></span>|



