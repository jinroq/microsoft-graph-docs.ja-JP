---
title: nonEapAuthenticationMethodForEapTtlsType 列挙型
description: 認証の非 EAP メソッドです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f14c98118541e6eeb6cb48fd54ac3fb69a722b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425597"
---
# <a name="noneapauthenticationmethodforeapttlstype-enum-type"></a><span data-ttu-id="7ad79-103">nonEapAuthenticationMethodForEapTtlsType 列挙型</span><span class="sxs-lookup"><span data-stu-id="7ad79-103">nonEapAuthenticationMethodForEapTtlsType enum type</span></span>

> <span data-ttu-id="7ad79-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7ad79-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7ad79-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ad79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ad79-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ad79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ad79-107">認証の非 EAP メソッドです。</span><span class="sxs-lookup"><span data-stu-id="7ad79-107">Non-EAP methods for authentication.</span></span>

## <a name="members"></a><span data-ttu-id="7ad79-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7ad79-108">Members</span></span>
|<span data-ttu-id="7ad79-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="7ad79-109">Member</span></span>|<span data-ttu-id="7ad79-110">値</span><span class="sxs-lookup"><span data-stu-id="7ad79-110">Value</span></span>|<span data-ttu-id="7ad79-111">説明</span><span class="sxs-lookup"><span data-stu-id="7ad79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ad79-112">unencryptedPassword</span><span class="sxs-lookup"><span data-stu-id="7ad79-112">unencryptedPassword</span></span>|<span data-ttu-id="7ad79-113">0</span><span class="sxs-lookup"><span data-stu-id="7ad79-113">0</span></span>|<span data-ttu-id="7ad79-114">暗号化されていないパスワード (PAP) です。</span><span class="sxs-lookup"><span data-stu-id="7ad79-114">Unencrypted password (PAP).</span></span>|
|<span data-ttu-id="7ad79-115">challengeHandshakeAuthenticationProtocol</span><span class="sxs-lookup"><span data-stu-id="7ad79-115">challengeHandshakeAuthenticationProtocol</span></span>|<span data-ttu-id="7ad79-116">1</span><span class="sxs-lookup"><span data-stu-id="7ad79-116">1</span></span>|<span data-ttu-id="7ad79-117">チャレンジ ハンドシェイク認証プロトコル (CHAP)。</span><span class="sxs-lookup"><span data-stu-id="7ad79-117">Challenge Handshake Authentication Protocol (CHAP).</span></span>|
|<span data-ttu-id="7ad79-118">microsoftChap</span><span class="sxs-lookup"><span data-stu-id="7ad79-118">microsoftChap</span></span>|<span data-ttu-id="7ad79-119">2</span><span class="sxs-lookup"><span data-stu-id="7ad79-119">2</span></span>| <span data-ttu-id="7ad79-120">Microsoft CHAP (MS-CHAP)。</span><span class="sxs-lookup"><span data-stu-id="7ad79-120">Microsoft CHAP (MS-CHAP).</span></span>|
|<span data-ttu-id="7ad79-121">microsoftChapVersionTwo</span><span class="sxs-lookup"><span data-stu-id="7ad79-121">microsoftChapVersionTwo</span></span>|<span data-ttu-id="7ad79-122">3</span><span class="sxs-lookup"><span data-stu-id="7ad79-122">3</span></span>|<span data-ttu-id="7ad79-123">Microsoft CHAP バージョン 2 (MS-CHAP v2)。</span><span class="sxs-lookup"><span data-stu-id="7ad79-123">Microsoft CHAP Version 2 (MS-CHAP v2).</span></span>|




