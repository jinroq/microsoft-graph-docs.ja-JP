---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef7f3a636f86139aa5107d1213e6cfe3d173dc51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001363"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="57c28-103">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="57c28-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="57c28-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57c28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57c28-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="57c28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57c28-106">FirewallCertificateRevocationListCheckMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="57c28-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="57c28-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="57c28-107">Members</span></span>
|<span data-ttu-id="57c28-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="57c28-108">Member</span></span>|<span data-ttu-id="57c28-109">値</span><span class="sxs-lookup"><span data-stu-id="57c28-109">Value</span></span>|<span data-ttu-id="57c28-110">説明</span><span class="sxs-lookup"><span data-stu-id="57c28-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57c28-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="57c28-111">deviceDefault</span></span>|<span data-ttu-id="57c28-112">.0</span><span class="sxs-lookup"><span data-stu-id="57c28-112">0</span></span>|<span data-ttu-id="57c28-113">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="57c28-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="57c28-114">none</span><span class="sxs-lookup"><span data-stu-id="57c28-114">none</span></span>|<span data-ttu-id="57c28-115">1-d</span><span class="sxs-lookup"><span data-stu-id="57c28-115">1</span></span>|<span data-ttu-id="57c28-116">証明書失効リストをチェックしない</span><span class="sxs-lookup"><span data-stu-id="57c28-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="57c28-117">再試行</span><span class="sxs-lookup"><span data-stu-id="57c28-117">attempt</span></span>|<span data-ttu-id="57c28-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="57c28-118">2</span></span>|<span data-ttu-id="57c28-119">証明書がチェックで確認されている場合にのみ、CRL の確認と許可を試行します。</span><span class="sxs-lookup"><span data-stu-id="57c28-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="57c28-120">要する</span><span class="sxs-lookup"><span data-stu-id="57c28-120">require</span></span>|<span data-ttu-id="57c28-121">1/3</span><span class="sxs-lookup"><span data-stu-id="57c28-121">3</span></span>|<span data-ttu-id="57c28-122">証明書を許可する前に、正常な CRL チェックを必要とする</span><span class="sxs-lookup"><span data-stu-id="57c28-122">Require a successful CRL check before allowing a certificate</span></span>|





