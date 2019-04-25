---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: firewallCertificateRevocationListCheckMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a475f32d4572b0aa8ed2a52befc7a58eb6077253
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541166"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="a342c-103">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a342c-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="a342c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a342c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a342c-105">firewallCertificateRevocationListCheckMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="a342c-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="a342c-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a342c-106">Members</span></span>
|<span data-ttu-id="a342c-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a342c-107">Member</span></span>|<span data-ttu-id="a342c-108">値</span><span class="sxs-lookup"><span data-stu-id="a342c-108">Value</span></span>|<span data-ttu-id="a342c-109">説明</span><span class="sxs-lookup"><span data-stu-id="a342c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a342c-110">devicedefault</span><span class="sxs-lookup"><span data-stu-id="a342c-110">deviceDefault</span></span>|<span data-ttu-id="a342c-111">.0</span><span class="sxs-lookup"><span data-stu-id="a342c-111">0</span></span>|<span data-ttu-id="a342c-112">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="a342c-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="a342c-113">なし</span><span class="sxs-lookup"><span data-stu-id="a342c-113">none</span></span>|<span data-ttu-id="a342c-114">1 </span><span class="sxs-lookup"><span data-stu-id="a342c-114">1</span></span>|<span data-ttu-id="a342c-115">証明書失効リストをチェックしない</span><span class="sxs-lookup"><span data-stu-id="a342c-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="a342c-116">再試行</span><span class="sxs-lookup"><span data-stu-id="a342c-116">attempt</span></span>|<span data-ttu-id="a342c-117">2 </span><span class="sxs-lookup"><span data-stu-id="a342c-117">2</span></span>|<span data-ttu-id="a342c-118">証明書がチェックで確認されている場合にのみ、CRL の確認と許可を試行します。</span><span class="sxs-lookup"><span data-stu-id="a342c-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="a342c-119">要する</span><span class="sxs-lookup"><span data-stu-id="a342c-119">require</span></span>|<span data-ttu-id="a342c-120">3 </span><span class="sxs-lookup"><span data-stu-id="a342c-120">3</span></span>|<span data-ttu-id="a342c-121">証明書を許可する前に、正常な CRL チェックを必要とする</span><span class="sxs-lookup"><span data-stu-id="a342c-121">Require a successful CRL check before allowing a certificate</span></span>|



