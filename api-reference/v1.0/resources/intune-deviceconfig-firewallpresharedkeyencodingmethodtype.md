---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: FirewallPreSharedKeyEncodingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ad59a11aec2fbf715657de95eb3aafc778da43a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947828"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="c6e73-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c6e73-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="c6e73-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6e73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6e73-105">FirewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="c6e73-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="c6e73-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="c6e73-106">Members</span></span>
|<span data-ttu-id="c6e73-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="c6e73-107">Member</span></span>|<span data-ttu-id="c6e73-108">値</span><span class="sxs-lookup"><span data-stu-id="c6e73-108">Value</span></span>|<span data-ttu-id="c6e73-109">説明</span><span class="sxs-lookup"><span data-stu-id="c6e73-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6e73-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="c6e73-110">deviceDefault</span></span>|<span data-ttu-id="c6e73-111">0</span><span class="sxs-lookup"><span data-stu-id="c6e73-111">0</span></span>|<span data-ttu-id="c6e73-112">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="c6e73-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="c6e73-113">none</span><span class="sxs-lookup"><span data-stu-id="c6e73-113">none</span></span>|<span data-ttu-id="c6e73-114">1</span><span class="sxs-lookup"><span data-stu-id="c6e73-114">1</span></span>|<span data-ttu-id="c6e73-115">事前共有キーはエンコードされません。</span><span class="sxs-lookup"><span data-stu-id="c6e73-115">Preshared key is not encoded.</span></span> <span data-ttu-id="c6e73-116">ワイド文字形式で保存される代わりに、</span><span class="sxs-lookup"><span data-stu-id="c6e73-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="c6e73-117">utF8</span><span class="sxs-lookup"><span data-stu-id="c6e73-117">utF8</span></span>|<span data-ttu-id="c6e73-118">2</span><span class="sxs-lookup"><span data-stu-id="c6e73-118">2</span></span>|<span data-ttu-id="c6e73-119">UTF-8 を使用して事前共有キーをエンコードします。</span><span class="sxs-lookup"><span data-stu-id="c6e73-119">Encode the preshared key using UTF-8</span></span>|



