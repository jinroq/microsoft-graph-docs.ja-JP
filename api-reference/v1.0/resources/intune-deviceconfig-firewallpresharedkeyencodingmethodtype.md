---
title: firewallPreSharedKeyEncodingMethodType 列挙型
description: FirewallPreSharedKeyEncodingMethod に指定できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bba6033985f2b960a272134614d98acc7203a9d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871751"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="02293-103">firewallPreSharedKeyEncodingMethodType 列挙型</span><span class="sxs-lookup"><span data-stu-id="02293-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="02293-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="02293-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02293-105">FirewallPreSharedKeyEncodingMethod に指定できる値</span><span class="sxs-lookup"><span data-stu-id="02293-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="02293-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="02293-106">Members</span></span>
|<span data-ttu-id="02293-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="02293-107">Member</span></span>|<span data-ttu-id="02293-108">値</span><span class="sxs-lookup"><span data-stu-id="02293-108">Value</span></span>|<span data-ttu-id="02293-109">説明</span><span class="sxs-lookup"><span data-stu-id="02293-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02293-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="02293-110">deviceDefault</span></span>|<span data-ttu-id="02293-111">0</span><span class="sxs-lookup"><span data-stu-id="02293-111">0</span></span>|<span data-ttu-id="02293-112">Intune で構成されている値は、デバイスのユーザーが設定した既定値をオーバーライドしない場合</span><span class="sxs-lookup"><span data-stu-id="02293-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="02293-113">none</span><span class="sxs-lookup"><span data-stu-id="02293-113">none</span></span>|<span data-ttu-id="02293-114">1</span><span class="sxs-lookup"><span data-stu-id="02293-114">1</span></span>|<span data-ttu-id="02293-115">事前共有キーはエンコードされません。</span><span class="sxs-lookup"><span data-stu-id="02293-115">Preshared key is not encoded.</span></span> <span data-ttu-id="02293-116">ワイド文字形式で保存される代わりに、</span><span class="sxs-lookup"><span data-stu-id="02293-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="02293-117">utF8</span><span class="sxs-lookup"><span data-stu-id="02293-117">utF8</span></span>|<span data-ttu-id="02293-118">2</span><span class="sxs-lookup"><span data-stu-id="02293-118">2</span></span>|<span data-ttu-id="02293-119">UTF-8 を使用して事前共有キーをエンコードします。</span><span class="sxs-lookup"><span data-stu-id="02293-119">Encode the preshared key using UTF-8</span></span>|



