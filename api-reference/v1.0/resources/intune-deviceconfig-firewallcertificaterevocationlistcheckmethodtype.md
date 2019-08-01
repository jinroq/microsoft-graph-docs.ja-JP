---
title: firewallCertificateRevocationListCheckMethodType 列挙型
description: FirewallCertificateRevocationListCheckMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7c5fa3baaeb3d24bc902d733a6c6462fbcf70f33
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028302"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="def44-103">firewallCertificateRevocationListCheckMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="def44-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="def44-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="def44-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="def44-105">FirewallCertificateRevocationListCheckMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="def44-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="def44-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="def44-106">Members</span></span>
|<span data-ttu-id="def44-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="def44-107">Member</span></span>|<span data-ttu-id="def44-108">値</span><span class="sxs-lookup"><span data-stu-id="def44-108">Value</span></span>|<span data-ttu-id="def44-109">説明</span><span class="sxs-lookup"><span data-stu-id="def44-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="def44-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="def44-110">deviceDefault</span></span>|<span data-ttu-id="def44-111">.0</span><span class="sxs-lookup"><span data-stu-id="def44-111">0</span></span>|<span data-ttu-id="def44-112">Intune によって構成された値がない。ユーザーが構成したデバイスの既定値を上書きしない</span><span class="sxs-lookup"><span data-stu-id="def44-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="def44-113">none</span><span class="sxs-lookup"><span data-stu-id="def44-113">none</span></span>|<span data-ttu-id="def44-114">1-d</span><span class="sxs-lookup"><span data-stu-id="def44-114">1</span></span>|<span data-ttu-id="def44-115">証明書失効リストをチェックしない</span><span class="sxs-lookup"><span data-stu-id="def44-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="def44-116">再試行</span><span class="sxs-lookup"><span data-stu-id="def44-116">attempt</span></span>|<span data-ttu-id="def44-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="def44-117">2</span></span>|<span data-ttu-id="def44-118">証明書がチェックで確認されている場合にのみ、CRL の確認と許可を試行します。</span><span class="sxs-lookup"><span data-stu-id="def44-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="def44-119">要する</span><span class="sxs-lookup"><span data-stu-id="def44-119">require</span></span>|<span data-ttu-id="def44-120">1/3</span><span class="sxs-lookup"><span data-stu-id="def44-120">3</span></span>|<span data-ttu-id="def44-121">証明書を許可する前に、正常な CRL チェックを必要とする</span><span class="sxs-lookup"><span data-stu-id="def44-121">Require a successful CRL check before allowing a certificate</span></span>|



