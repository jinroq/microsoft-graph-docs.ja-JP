---
title: nonEapAuthenticationMethodForEapTtlsType 列挙型
description: 認証の非 EAP メソッドです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 146eaa57ddc79eb930a0334ee1c227c1541c8609
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952686"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a><span data-ttu-id="d6c4a-103">nonEapAuthenticationMethodForEapTtlsType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d6c4a-103">nonEapAuthenticationMethodForEapTtlsType enum type</span></span>

> <span data-ttu-id="d6c4a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6c4a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6c4a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6c4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6c4a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d6c4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6c4a-107">認証の非 EAP メソッドです。</span><span class="sxs-lookup"><span data-stu-id="d6c4a-107">Non-EAP methods for authentication.</span></span>
## <a name="members"></a><span data-ttu-id="d6c4a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6c4a-108">Members</span></span>
|<span data-ttu-id="d6c4a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="d6c4a-109">Member</span></span>|<span data-ttu-id="d6c4a-110">値</span><span class="sxs-lookup"><span data-stu-id="d6c4a-110">Value</span></span>|<span data-ttu-id="d6c4a-111">説明</span><span class="sxs-lookup"><span data-stu-id="d6c4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c4a-112">unencryptedPassword</span><span class="sxs-lookup"><span data-stu-id="d6c4a-112">unencryptedPassword</span></span>|<span data-ttu-id="d6c4a-113">0</span><span class="sxs-lookup"><span data-stu-id="d6c4a-113">0</span></span>|<span data-ttu-id="d6c4a-114">暗号化されていないパスワード (PAP) です。</span><span class="sxs-lookup"><span data-stu-id="d6c4a-114">Unencrypted password (PAP).</span></span>|
|<span data-ttu-id="d6c4a-115">challengeHandshakeAuthenticationProtocol</span><span class="sxs-lookup"><span data-stu-id="d6c4a-115">challengeHandshakeAuthenticationProtocol</span></span>|<span data-ttu-id="d6c4a-116">1</span><span class="sxs-lookup"><span data-stu-id="d6c4a-116">1</span></span>|<span data-ttu-id="d6c4a-117">チャレンジ ハンドシェイク認証プロトコル (CHAP)。</span><span class="sxs-lookup"><span data-stu-id="d6c4a-117">Challenge Handshake Authentication Protocol (CHAP).</span></span>|
|<span data-ttu-id="d6c4a-118">microsoftChap</span><span class="sxs-lookup"><span data-stu-id="d6c4a-118">microsoftChap</span></span>|<span data-ttu-id="d6c4a-119">2</span><span class="sxs-lookup"><span data-stu-id="d6c4a-119">2</span></span>| <span data-ttu-id="d6c4a-120">Microsoft CHAP (MS-CHAP)。</span><span class="sxs-lookup"><span data-stu-id="d6c4a-120">Microsoft CHAP (MS-CHAP).</span></span>|
|<span data-ttu-id="d6c4a-121">microsoftChapVersionTwo</span><span class="sxs-lookup"><span data-stu-id="d6c4a-121">microsoftChapVersionTwo</span></span>|<span data-ttu-id="d6c4a-122">3</span><span class="sxs-lookup"><span data-stu-id="d6c4a-122">3</span></span>|<span data-ttu-id="d6c4a-123">Microsoft CHAP バージョン 2 (MS-CHAP v2)。</span><span class="sxs-lookup"><span data-stu-id="d6c4a-123">Microsoft CHAP Version 2 (MS-CHAP v2).</span></span>|





