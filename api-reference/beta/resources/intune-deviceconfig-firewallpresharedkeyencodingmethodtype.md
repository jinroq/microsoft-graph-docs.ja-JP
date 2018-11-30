---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: FirewallPreSharedKeyEncodingMethod に指定できる値
ms.openlocfilehash: 3f6d4a88ec4f0296bfd0d35f30695ddae14d4c95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066535"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="62ff8-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="62ff8-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="62ff8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="62ff8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62ff8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62ff8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62ff8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="62ff8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62ff8-107">FirewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="62ff8-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="62ff8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="62ff8-108">Members</span></span>
|<span data-ttu-id="62ff8-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="62ff8-109">Member</span></span>|<span data-ttu-id="62ff8-110">値</span><span class="sxs-lookup"><span data-stu-id="62ff8-110">Value</span></span>|<span data-ttu-id="62ff8-111">説明</span><span class="sxs-lookup"><span data-stu-id="62ff8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62ff8-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="62ff8-112">deviceDefault</span></span>|<span data-ttu-id="62ff8-113">0</span><span class="sxs-lookup"><span data-stu-id="62ff8-113">0</span></span>|<span data-ttu-id="62ff8-114">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="62ff8-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="62ff8-115">none</span><span class="sxs-lookup"><span data-stu-id="62ff8-115">none</span></span>|<span data-ttu-id="62ff8-116">1</span><span class="sxs-lookup"><span data-stu-id="62ff8-116">1</span></span>|<span data-ttu-id="62ff8-117">事前共有キーはエンコードされません。</span><span class="sxs-lookup"><span data-stu-id="62ff8-117">Preshared key is not encoded.</span></span> <span data-ttu-id="62ff8-118">ワイド文字形式で保存される代わりに、</span><span class="sxs-lookup"><span data-stu-id="62ff8-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="62ff8-119">utF8</span><span class="sxs-lookup"><span data-stu-id="62ff8-119">utF8</span></span>|<span data-ttu-id="62ff8-120">2</span><span class="sxs-lookup"><span data-stu-id="62ff8-120">2</span></span>|<span data-ttu-id="62ff8-121">UTF-8 を使用して事前共有キーをエンコードします。</span><span class="sxs-lookup"><span data-stu-id="62ff8-121">Encode the preshared key using UTF-8</span></span>|





