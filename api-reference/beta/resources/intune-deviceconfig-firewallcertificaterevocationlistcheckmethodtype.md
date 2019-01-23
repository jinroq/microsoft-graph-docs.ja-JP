---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4585c30c0a910befd8df8482636916af9ad9c0d6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396414"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="263ca-103">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="263ca-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="263ca-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="263ca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="263ca-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="263ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="263ca-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="263ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="263ca-107">FirewallCertificateRevocationListCheckMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="263ca-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="263ca-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="263ca-108">Members</span></span>
|<span data-ttu-id="263ca-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="263ca-109">Member</span></span>|<span data-ttu-id="263ca-110">値</span><span class="sxs-lookup"><span data-stu-id="263ca-110">Value</span></span>|<span data-ttu-id="263ca-111">説明</span><span class="sxs-lookup"><span data-stu-id="263ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="263ca-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="263ca-112">deviceDefault</span></span>|<span data-ttu-id="263ca-113">0</span><span class="sxs-lookup"><span data-stu-id="263ca-113">0</span></span>|<span data-ttu-id="263ca-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="263ca-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="263ca-115">none</span><span class="sxs-lookup"><span data-stu-id="263ca-115">none</span></span>|<span data-ttu-id="263ca-116">1</span><span class="sxs-lookup"><span data-stu-id="263ca-116">1</span></span>|<span data-ttu-id="263ca-117">証明書失効リストをチェックしません。</span><span class="sxs-lookup"><span data-stu-id="263ca-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="263ca-118">試行</span><span class="sxs-lookup"><span data-stu-id="263ca-118">attempt</span></span>|<span data-ttu-id="263ca-119">2</span><span class="sxs-lookup"><span data-stu-id="263ca-119">2</span></span>|<span data-ttu-id="263ca-120">CRL チェックを試みるし、チェックして、証明書が確認される場合にのみ証明書を許可します。</span><span class="sxs-lookup"><span data-stu-id="263ca-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="263ca-121">必要</span><span class="sxs-lookup"><span data-stu-id="263ca-121">require</span></span>|<span data-ttu-id="263ca-122">3</span><span class="sxs-lookup"><span data-stu-id="263ca-122">3</span></span>|<span data-ttu-id="263ca-123">証明書を許可する前に成功した CRL チェックが必要</span><span class="sxs-lookup"><span data-stu-id="263ca-123">Require a successful CRL check before allowing a certificate</span></span>|




