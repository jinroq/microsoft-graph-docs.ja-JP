---
title: vpnAuthenticationMethod 列挙型
description: VPN 認証方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58cb031abbcf520a8a970aa80bacd2390b860343
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367793"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="86c01-103">vpnAuthenticationMethod 列挙型</span><span class="sxs-lookup"><span data-stu-id="86c01-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="86c01-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86c01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86c01-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86c01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86c01-106">VPN 認証方法。</span><span class="sxs-lookup"><span data-stu-id="86c01-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="86c01-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="86c01-107">Members</span></span>
|<span data-ttu-id="86c01-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="86c01-108">Member</span></span>|<span data-ttu-id="86c01-109">値</span><span class="sxs-lookup"><span data-stu-id="86c01-109">Value</span></span>|<span data-ttu-id="86c01-110">説明</span><span class="sxs-lookup"><span data-stu-id="86c01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86c01-111">certificate</span><span class="sxs-lookup"><span data-stu-id="86c01-111">certificate</span></span>|<span data-ttu-id="86c01-112">.0</span><span class="sxs-lookup"><span data-stu-id="86c01-112">0</span></span>|<span data-ttu-id="86c01-113">証明書を使用して認証します。</span><span class="sxs-lookup"><span data-stu-id="86c01-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="86c01-114">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="86c01-114">usernameAndPassword</span></span>|<span data-ttu-id="86c01-115">1-d</span><span class="sxs-lookup"><span data-stu-id="86c01-115">1</span></span>|<span data-ttu-id="86c01-116">認証にユーザー名とパスワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="86c01-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="86c01-117">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="86c01-117">sharedSecret</span></span>|<span data-ttu-id="86c01-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="86c01-118">2</span></span>|<span data-ttu-id="86c01-119">認証に共有シークレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="86c01-119">Use Shared Secret for Authentication.</span></span>  <span data-ttu-id="86c01-120">IOS IKEv2 に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="86c01-120">Only valid for iOS IKEv2.</span></span>|
|<span data-ttu-id="86c01-121">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="86c01-121">derivedCredential</span></span>|<span data-ttu-id="86c01-122">1/3</span><span class="sxs-lookup"><span data-stu-id="86c01-122">3</span></span>|<span data-ttu-id="86c01-123">認証に派生した資格情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="86c01-123">Use Derived Credential for Authentication.</span></span>  <span data-ttu-id="86c01-124">IOS に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="86c01-124">Only valid for iOS.</span></span>|



