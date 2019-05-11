---
title: vpnAuthenticationMethod 列挙型
description: VPN 認証方法。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f75c7ec53f406e7f998a89faa8d1dabf4c650de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944622"
---
# <a name="vpnauthenticationmethod-enum-type"></a><span data-ttu-id="5300f-103">vpnAuthenticationMethod 列挙型</span><span class="sxs-lookup"><span data-stu-id="5300f-103">vpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="5300f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5300f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5300f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5300f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5300f-106">VPN 認証方法。</span><span class="sxs-lookup"><span data-stu-id="5300f-106">VPN Authentication Method.</span></span>

## <a name="members"></a><span data-ttu-id="5300f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5300f-107">Members</span></span>
|<span data-ttu-id="5300f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5300f-108">Member</span></span>|<span data-ttu-id="5300f-109">値</span><span class="sxs-lookup"><span data-stu-id="5300f-109">Value</span></span>|<span data-ttu-id="5300f-110">説明</span><span class="sxs-lookup"><span data-stu-id="5300f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5300f-111">certificate</span><span class="sxs-lookup"><span data-stu-id="5300f-111">certificate</span></span>|<span data-ttu-id="5300f-112">.0</span><span class="sxs-lookup"><span data-stu-id="5300f-112">0</span></span>|<span data-ttu-id="5300f-113">証明書を使用して認証します。</span><span class="sxs-lookup"><span data-stu-id="5300f-113">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="5300f-114">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="5300f-114">usernameAndPassword</span></span>|<span data-ttu-id="5300f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5300f-115">1</span></span>|<span data-ttu-id="5300f-116">認証にユーザー名とパスワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="5300f-116">Use username and password for authentication.</span></span>|
|<span data-ttu-id="5300f-117">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="5300f-117">derivedCredential</span></span>|<span data-ttu-id="5300f-118">1/3</span><span class="sxs-lookup"><span data-stu-id="5300f-118">3</span></span>|<span data-ttu-id="5300f-119">認証に派生した資格情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="5300f-119">Use Derived Credential for Authentication.</span></span>  <span data-ttu-id="5300f-120">IOS に対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="5300f-120">Only valid for iOS.</span></span>|




