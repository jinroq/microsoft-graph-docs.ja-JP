---
title: emailCertificateType 列挙型
description: 電子メールの署名と暗号化に対してサポートされている証明書ソース。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c6c4a6943fada88dc9a30c9e81d45705153dfde1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357188"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="a6ad0-103">emailCertificateType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a6ad0-103">emailCertificateType enum type</span></span>

> <span data-ttu-id="a6ad0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6ad0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6ad0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6ad0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6ad0-106">電子メールの署名と暗号化に対してサポートされている証明書ソース。</span><span class="sxs-lookup"><span data-stu-id="a6ad0-106">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="a6ad0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6ad0-107">Members</span></span>
|<span data-ttu-id="a6ad0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a6ad0-108">Member</span></span>|<span data-ttu-id="a6ad0-109">値</span><span class="sxs-lookup"><span data-stu-id="a6ad0-109">Value</span></span>|<span data-ttu-id="a6ad0-110">説明</span><span class="sxs-lookup"><span data-stu-id="a6ad0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6ad0-111">none</span><span class="sxs-lookup"><span data-stu-id="a6ad0-111">none</span></span>|<span data-ttu-id="a6ad0-112">.0</span><span class="sxs-lookup"><span data-stu-id="a6ad0-112">0</span></span>|<span data-ttu-id="a6ad0-113">証明書をソースとして使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="a6ad0-113">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="a6ad0-114">certificate</span><span class="sxs-lookup"><span data-stu-id="a6ad0-114">certificate</span></span>|<span data-ttu-id="a6ad0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a6ad0-115">1</span></span>|<span data-ttu-id="a6ad0-116">証明書ソースに証明書を使用します。</span><span class="sxs-lookup"><span data-stu-id="a6ad0-116">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="a6ad0-117">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="a6ad0-117">derivedCredential</span></span>|<span data-ttu-id="a6ad0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a6ad0-118">2</span></span>|<span data-ttu-id="a6ad0-119">証明書ソースに派生した資格情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="a6ad0-119">Use a derived credential for certificate source.</span></span>|



